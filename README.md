# generator-alexa-skill [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url]

> A [Yeoman](http://yeoman.io) generator for scaffolding an Alexa Skill for AWS Lambda

## Installation

```bash
npm install -g yo generator-alexa-skill
```

## Generating an Alexa Skill

```bash
yo alexa-skill
```

This creates a brand new Alexa Skill, add your logic into `lib/<skill-name>.js` and tests into `test/<skill-name>.spec.js`.

## Deploying to AWS Lambda

To build the skill for use on AWS Lambda:

```bash
npm run prepublish
```

This creates `dist/alexa-skill-<skill-name>.js`, copy and paste the contents of the file into your AWS Lambda function. The script exports a single handler called `<skill-name>`, this is the handler name you configure your AWS Lambda function to use.

## License

MIT
