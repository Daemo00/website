To use this module, you need to add an input field with the
``js_website_autocomplete`` class, such as in the below format:

.. code:: xml

    <input type="text"
           class="js_website_autocomplete"
           data-query-field="name"
           data-display-field="name"
           data-value-field="id"
           data-limit="10"
           data-domain='[["website_published", "=", true]]'
           data-model="product.template"
           />

Following is a breakdown of the available attributes & their defaults:

+--------------------+---------------------------------------------+---------------+----------+
|  Attribute         |  Description                                |  Default      | Required |
+====================+=============================================+===============+==========+
| data-model         | Model name to query                         |               | True     |
+--------------------+---------------------------------------------+---------------+----------+
| data-query-field   | Field to query when searching               | name          | False    |
+--------------------+---------------------------------------------+---------------+----------+
| data-display-field | Field to display                            | query-field   | False    |
+--------------------+---------------------------------------------+---------------+----------+
| data-value-field   | Field to use as form value                  | display-field | False    |
+--------------------+---------------------------------------------+---------------+----------+
| data-limit         | Limit results to this many                  | 10            | False    |
+--------------------+---------------------------------------------+---------------+----------+
| data-domain        | Additional domain for query                 | []            | False    |
+--------------------+---------------------------------------------+---------------+----------+
