  appsmith:
    image: appsmith/appsmith-ce
    restart: always
    volumes:
      - ./stacks:/appsmith-stacks
    environment:
     - VER=1
    links:
      - mongo_dev:mongo
    stdin_open: true
    tty: true
