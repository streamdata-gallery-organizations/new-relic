---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Add Alerts Plugins Conditions Policies Policy  . Format
  version: 1.0.0
  description: |-
    This API endpoint allows you to create Plugins conditions for your alert policies.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on creating conditions for plugins.

    All fields are required except for ???runbook_url???, ???enabled??? (defaults to false).

    name: A title for your condition.

    enabled: The status of your condition (optional).

    entities: An array of instance IDs associated with your condition.

    metric_description: A title for the metric to display in notifications.

    metric: The metric to evaluate on.

    value_function: min, max, average, sample_size, total, percent

    runbook_url: Runbook URL to display in notifications (optional).

    terms[duration] (in minutes): 5, 10, 15, 30, 60, 120.

    terms[operator]: above, below, equal.

    terms[priority]: critical, warning.

    terms[threshold]: Must be 0 or greater.

    terms[time_function]: all, any.

    plugin[id]: The ID of the plugin.

    plugin[guid]: The GUID of the plugin.
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts_plugins_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Plugins Conditions Policies Policy  . Format
      description: |-
        This API endpoint allows you to create Plugins conditions for your alert policies.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on creating conditions for plugins.

        All fields are required except for ???runbook_url???, ???enabled??? (defaults to false).

        name: A title for your condition.

        enabled: The status of your condition (optional).

        entities: An array of instance IDs associated with your condition.

        metric_description: A title for the metric to display in notifications.

        metric: The metric to evaluate on.

        value_function: min, max, average, sample_size, total, percent

        runbook_url: Runbook URL to display in notifications (optional).

        terms[duration] (in minutes): 5, 10, 15, 30, 60, 120.

        terms[operator]: above, below, equal.

        terms[priority]: critical, warning.

        terms[threshold]: Must be 0 or greater.

        terms[time_function]: all, any.

        plugin[id]: The ID of the plugin.

        plugin[guid]: The GUID of the plugin.
      operationId: postAlertsPluginsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-plugins-conditionspoliciespolicy-id-format-post
      parameters:
      - in: body
        name: plugins_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
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