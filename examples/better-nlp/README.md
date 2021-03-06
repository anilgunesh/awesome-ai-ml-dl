# Better NLP

This is a wrapper program/library that encapsulates a couple of NLP libraries that are popular among the AI and ML communities.

Examples have been used to illustrate the usage as much as possible. Not all the APIs of the underlying libraries have been covered.

The idea is to keep the API language as high-level as possible, so its easier to use it easily and stays human-readable.

Libraries / frameworks covered:

- SpaCy
- Textacy
- Rasa NLU

## Requirements

- Python 3.7.x or higher
- Docker (optional)
- Diskspace: 2-3GB

## Installation

Setup an environment needed to be able to run these programs without having to worry about the dependencies they use.

Please be aware that even though we are install only a few components, the installation process takes some time (irrespective if you are running in via your local environment or inside a docker container). Give it about 20-30 minutes depending on network bandwidth and overall machine performance.

### Local environment

For the brave at heart, install the dependencies in your local environment.

#### Linux

```
./install-linux.sh
```

#### MacOS

```
./install-macos.sh
```

Alternatively please refer to the **Docker environment** section.

#### Windows

In principle, the `install-linux.sh` script should work in the `cygwin` or `git bash` environments - although it has not been tested, please raise PR with fixes if any. Alternatively please refer to the **Docker environment** section.

### Docker environment

Build a docker image with the necessary dependencies:

```
    ./buildDockerImage.sh
```

Run the docker container to start running the programs:

```
    ./runDockerImage.sh
```

## Example code

### Extract noun chunks from text

```
    python3 extract-noun-chunks-from-text.py
```

### Extracts facts from text

```
    python3 gather-facts-from-text.py
```

### Extracts entities from text

```
    python3 extract-entities-from-text.py            
```

### Obfuscate details from text for privacy

```
    python3 obfuscate-privacy-details-in-the-text.py
```