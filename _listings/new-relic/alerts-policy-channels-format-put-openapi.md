---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Put Alerts Policy Channels. Format
  version: 1.0.0
  description: |-
    This API endpoint updates policy/channel associations.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on updating notification channels with policies.
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
  /alerts_plugins_conditions/{id}.{format}:
    put:
      summary: Put Alerts Plugins Conditions  . Format
      description: |-
        This API endpoint allows you to update Plugins conditions for your alert policies.

        Note: Admin User???s API Key is required.

        See Alerts Plugins Conditions &gt; Create for an explanation of the field values ued in this command or the online document on
        updating conditions for plugins.
      operationId: putAlertsPluginsConditions.Format
      x-api-path-slug: alerts-plugins-conditionsid-format-put
      parameters:
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      - in: body
        name: plugins_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - ""
      - .
      - Format
  /alerts_plugins_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Plugins Conditions Condition  . Format
      description: |-
        This API endpoint allows you to delete Plugins conditions associated with your alert policy.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on deleting Plugins conditions.
      operationId: deleteAlertsPluginsConditionsCondition.Format
      x-api-path-slug: alerts-plugins-conditionscondition-id-format-delete
      parameters:
      - in: path
        name: condition_id
        description: Alerts condition ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_plugins_conditions.{format}:
    get:
      summary: Get Alerts Plugins Conditions. Format
      description: "This API endpoint allows you to list the Plugins conditions for
        your alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsPluginsConditions.Format
      x-api-path-slug: alerts-plugins-conditions-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      - in: query
        name: policy_id
        description: Alerts policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Plugins
      - Conditions.
      - Format
  /alerts_policy_channels.{format}:
    put:
      summary: Put Alerts Policy Channels. Format
      description: |-
        This API endpoint updates policy/channel associations.

        Note: Admin User???s API Key is required.

        See our documentation for a discussion on updating notification channels with policies.
      operationId: putAlertsPolicyChannels.Format
      x-api-path-slug: alerts-policy-channels-format-put
      parameters:
      - in: query
        name: channel_ids
        description: Channel IDs
        type: list
      - in: query
        name: policy_id
        description: Policy ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Policy
      - Channels.
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