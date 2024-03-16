# Mudey Server

## Introduction

Mudey Server is a Node.js package that provides functionality to generate Apache or Nginx virtual host configurations for web servers.

## Installation

To install Mudey Server globally, you can use npm:

```bash
npm install -g mudey-server
```

## Usage

### Command Line Interface

Mudey Server can be used via the command line interface (CLI) to generate virtual host configurations for Apache or Nginx.

```bash
mudey-server [options]
```

#### Options:

- `--apache`: Generate Apache virtual host configuration.
- `--nginx`: Generate Nginx virtual host configuration.
- `--routing`: Enable routing (for single-page applications).
- `--cache`: Enable caching.

### Example Usage:

Generate Apache virtual host configuration:

```bash
mudey-server --apache --routing --cache
```

Generate Nginx virtual host configuration:

```bash
mudey-server --nginx
```

## API

Mudey Server also provides an API for generating virtual host configurations programmatically.

### Functions:

#### `generateApacheVHost(domain, documentRoot, routing, cache)`

Generates Apache virtual host configuration.

- `domain`: Domain name for the virtual host.
- `documentRoot`: Document root directory.
- `routing`: Enable routing.
- `cache`: Enable caching.

#### `generateNginxVHost(domain, documentRoot, routing, cache)`

Generates Nginx virtual host configuration.

- `domain`: Domain name for the virtual host.
- `documentRoot`: Document root directory.
- `routing`: Enable routing.
- `cache`: Enable caching.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
