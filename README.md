# Workshop Stress Test

This repository is dedicated to stress testing the LEAP server.

## Project Overview

The project is designed to simulate high load and stress conditions for testing the performance and stability of the LEAP server.

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/mbchavez27/workshop-stress-test.git
cd workshop-stress-test
npm install
npm run dev
```

## Docker Setup

If you'd prefer to run the application using Docker, follow the steps below:

1. Build the Docker image:

```bash
docker build -t workshop-stress-test .
```

2. Run the Docker container:

```bash
docker run -p 3000:3000 workshop-stress-test
```

This will start the application and expose it on port 3000.

## Contributing

If you have suggestions or improvements, feel free to fork this repository, open issues, or submit pull requests.
