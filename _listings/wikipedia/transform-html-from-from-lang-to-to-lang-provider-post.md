---
swagger: "2.0"
info:
  title: Wikipedia
  description: This API provides cacheable and straightforward access to Wikimedia
    content and data, in machine-readable formats.
  termsOfService: https://wikimediafoundation.org/wiki/Terms_of_Use
  contact:
    name: the Wikimedia Services team
    url: http://mediawiki.org/wiki/REST_API
  version: v1
host: wikimedia.org
basePath: /api/rest_v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transform/html/from/{from_lang}/to/{to_lang}/{provider}:
    post:
      summary: Machine-translate content
      description: |-
        Fetches the machine translation for the posted content from the source
        to the destination language
      operationId: fetches-the-machine-translation-for-the-posted-content-from-the-sourceto-the-destination-languagesta
      parameters:
      - in: path
        name: from_lang
        description: The source language code
      - in: formData
        name: html
        description: The HTML content to translate
      - in: path
        name: provider
        description: The machine translation provider id
      - in: path
        name: to_lang
        description: The target language code
      responses:
        200:
          description: OK
      tags:
      - wiki
definitions:
  "":
    properties:
      type:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      detail:
        description: This is a default description.
        type: string
      instance:
        description: This is a default description.
        type: string
      items:
        description: This is a default description.
        type: string
      counter:
        description: This is a default description.
        type: string
      ids:
        description: This is a default description.
        type: string
      count:
        description: This is a default description.
        type: string
  absolute-bytes-difference:
    properties:
      items:
        description: This is a default description.
        type: parameters
  by-country:
    properties:
      items:
        description: This is a default description.
        type: parameters
  cx_dict:
    properties:
      source:
        description: This is a default description.
        type: parameters
      translations:
        description: This is a default description.
        type: parameters
  cx_languagepairs:
    properties:
      source:
        description: This is a default description.
        type: parameters
      target:
        description: This is a default description.
        type: parameters
  cx_list_tools:
    properties:
      tools:
        description: This is a default description.
        type: parameters
  cx_mt:
    properties:
      contents:
        description: This is a default description.
        type: parameters
  edited-pages:
    properties:
      items:
        description: This is a default description.
        type: parameters
  editors:
    properties:
      items:
        description: This is a default description.
        type: parameters
  edits:
    properties:
      items:
        description: This is a default description.
        type: parameters
  listing:
    properties:
      items:
        description: This is a default description.
        type: parameters
  net-bytes-difference:
    properties:
      items:
        description: This is a default description.
        type: parameters
  new-pages:
    properties:
      items:
        description: This is a default description.
        type: parameters
  new-registered-users:
    properties:
      items:
        description: This is a default description.
        type: parameters
  originalimage:
    properties:
      height:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
      width:
        description: This is a default description.
        type: parameters
  pagecounts-project:
    properties:
      items:
        description: This is a default description.
        type: parameters
  pageview-article:
    properties:
      items:
        description: This is a default description.
        type: parameters
  pageview-project:
    properties:
      items:
        description: This is a default description.
        type: parameters
  pageview-tops:
    properties:
      items:
        description: This is a default description.
        type: parameters
  problem:
    properties:
      detail:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  summary:
    properties:
      coordinates:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      dir:
        description: This is a default description.
        type: parameters
      displaytitle:
        description: This is a default description.
        type: parameters
      extract:
        description: This is a default description.
        type: parameters
      extract_html:
        description: This is a default description.
        type: parameters
      lang:
        description: This is a default description.
        type: parameters
      pageid:
        description: This is a default description.
        type: parameters
      timestamp:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  thumbnail:
    properties:
      height:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
      width:
        description: This is a default description.
        type: parameters
  top-edited-pages-by-abs-bytes-diff:
    properties:
      items:
        description: This is a default description.
        type: parameters
  top-edited-pages-by-edits:
    properties:
      items:
        description: This is a default description.
        type: parameters
  top-edited-pages-by-net-bytes-diff:
    properties:
      items:
        description: This is a default description.
        type: parameters
  top-editors-by-abs-bytes-diff:
    properties:
      items:
        description: This is a default description.
        type: parameters
  top-editors-by-edits:
    properties:
      items:
        description: This is a default description.
        type: parameters
  top-editors-by-net-bytes-diff:
    properties:
      items:
        description: This is a default description.
        type: parameters
  unique-devices:
    properties:
      items:
        description: This is a default description.
        type: parameters
x-collection-name: Wikipedia
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---