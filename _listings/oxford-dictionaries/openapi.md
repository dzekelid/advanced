---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 1
info:
  title: Oxford Dictionaries
  description: if-youre-looking-to-enhance-your-app-or-website-with-dictionary-data-dont-compromise-on-quality--the-oxford-dictionaries-api-offers-easy-and-intuitive-access-to-oxfords-dictionary-content-which-is-trusted-around-the-world--here-at-oxford-dictionaries-home-of-the-oed-we-love-words--thats-why-we-have-experienced-lexicographers-tracking-the-living-language-delving-deep-into-our-corpora-and-monitoring-a-wide-range-of-media-in-order-to-understand-how-words-are-being-used-and-how-language-is-evolving--this-research-is-used-by-our-editors-to-write-and-edit-dictionary-entries-and-translations-meaning-were-able-to-offer-uptodate-accurate-and-reliable-lexical-content-in-multiple-languages-
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /wordlist/{source_lang}/{filters_advanced}:
    get:
      summary: Retrieve list of words for category with advanced options
      description: Use this to apply more complex filters to the [list of words](documentation/glossary?term=wordlist).
        For example, you may only want to filter out words for which all [senses](documentation/glossary?term=sense)
        match the filter, or only its 'prime sense'. You can also filter by word length
        or match by substring (prefix).
      operationId: getWordlistSourceLangFiltersAdvanced
      x-api-path-slug: wordlistsource-langfilters-advanced-get
      parameters:
      - in: query
        name: exact
        description: If exact=true wordlist returns a list of entries that exactly
          matches the search string
      - in: query
        name: exclude
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: query
        name: exclude_prime_senses
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: query
        name: exclude_senses
        description: Semicolon separated list of parameters-value pairs (same as filters)
      - in: path
        name: filters_advanced
        description: 'Semicolon separated list of wordlist parameters, presented as
          value pairs: LexicalCategory, domains, regions, registers'
      - in: query
        name: limit
        description: Limit the number of results per response
      - in: query
        name: No Name
      - in: query
        name: offset
        description: Offset the start number of the result
      - in: query
        name: prefix
        description: Filter words that start with prefix parameter
      - in: query
        name: word_length
        description: Parameter to speficy the minimum (>), exact or maximum (5 - more
          than 5 chars; 5
      responses:
        200:
          description: OK
      tags:
      - Wordlist
      - Source
      - Lang
      - Filters
      - Advanced
---