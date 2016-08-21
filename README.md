# Using Docker Code Examples
## Chapter "User Docker in Development"

Amended version to make it work on Raspberry PI3, running Hypriot image 1.0.0

To build the docker image, execute the following command: ```docker build -t fxmartin/rpi-identidock .```

To run the example: ```docker run -d -p 5000:5000 fxmartin/rpi-identidock```

To test it: ```curl localhost:5000```

