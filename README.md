# Welcome to Google Translate Free API

This API is a robust translation service designed to help you with a variety of language-based features including direct translations, alternate translations, definitions, examples, transliterations, spelling suggestions, language detection, and highly relevant keyword suggestions.

## Features

Here are some key features of the API:

1. **Translation**: Get direct translations of vocabulary words or text fragments.
2. **Alternate Translations**: Extract an array of alternative translations of any text.
3. **Definitions**: Identify definitions of the keyword by word type (noun, verb, adjective, etc.).
4. **Examples**: Generate single-sentence examples containing the valid keyword.
5. **Transliteration**: Acquire the transliteration of a keyword string.
6. **Spelling Suggestions**: Get suggested corrections for spelling of vocabularies or texts.
7. **Language Detection**: Determine the text source language with precision score.
8. **Keyword Suggestions**: Discover suggested keywords for more detailed search.

Let's read the [documents](https://api.datpmt.com) before using it.
## Getting Started

These instructions will help you start working with the Google Translate Free API.

## Prerequisites

- Understand how to make GET requests to an API
- Have a tool for making HTTP requests (Postman, CURL, etc.)

## Using the API

Make GET requests to the following endpoints, replacing the parameters as necessary.

- To translate: `/api/v1/dictionary/translate` 
- For alternate translations: `/api/v1/dictionary/alternate_translations`
- For definitions: `/api/v1/dictionary/definitions`
- For examples: `/api/v1/dictionary/examples`
- For transliteration: `/api/v1/dictionary/transliteration`
- For spelling suggestions: `/api/v1/dictionary/suggest`
- For language detection: `/api/v1/dictionary/detection`
- For keyword suggestions: `/api/v1/dictionary/see_more`

## Running tests

To run tests, make GET requests to the API endpoints listed above using your chosen HTTP client.

## Author

* [datpmt](https://github.com/datpmt)

## License

This is a free application and must not be used for commercial purposes! DATPMT disclaims all litigation related to unauthorized use!
