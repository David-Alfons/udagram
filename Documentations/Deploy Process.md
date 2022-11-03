## Deploying Steps

steps:
      - checkout
      - node/install:
          node-version: '14.15'
      - run: node --version
      - aws-cli/setup
      - eb/setup
      - run:
          name: Install Back-End Dependencies
          command: 'npm run backend:install'
      - run:
          name: Back-End Build
          command: 'npm run backend:build'
      - run:
          name: Install Front-End Dependencies
          command: 'npm run frontend:install'
      - run:
          name: Front-End Build
          command: 'npm run frontend:build'
      - run:
          name: Deploy Backend
          command: 'npm run backend:deploy'
      - run:
          name: Deploy Frontend
          command: 'npm run frontend:deploy'