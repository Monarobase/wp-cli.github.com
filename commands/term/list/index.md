---
layout: default
title: 'wp term list'
display_global_parameters: true
---

`wp term list` - List terms in a taxonomy.

<small>Quick links: <a href="https://github.com/wp-cli/wp-cli/issues?q=is%3Aopen+label%3Acommand%3Aterm-list+sort%3Aupdated-desc">Github issues</a></small>

<hr />

### OPTIONS

&lt;taxonomy&gt;...
: List terms of one or more taxonomies

[\--&lt;field&gt;=&lt;value&gt;]
: Filter by one or more fields (see get_terms() $args parameter for a list of fields).

[\--field=&lt;field&gt;]
: Prints the value of a single field for each term.

[\--fields=&lt;fields&gt;]
: Limit the output to specific object fields.

[\--format=&lt;format&gt;]
: Accepted values: table, csv, json, count, yaml. Default: table

### AVAILABLE FIELDS

These fields will be displayed by default for each term:

* term_id
* term_taxonomy_id
* name
* slug
* description
* parent
* count

There are no optionally available fields.

### EXAMPLES

    wp term list category --format=csv

    wp term list post_tag --fields=name,slug



