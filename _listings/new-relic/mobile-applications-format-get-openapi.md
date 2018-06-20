---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 0
info:
  title: New Relic Get Mobile Applications. Format
  version: 1.0.0
  description: |-
    This API endpoint returns a list of the Mobile Applications associated with your New Relic account.

    MobileApplications can be filtered by their name, or by the application IDs.
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
      description: "This API endpoint allows you to create Plugins conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating conditions for plugins.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\nname: A title for your condition.\n\nenabled: The
        status of your condition (optional).\n\nentities: An array of instance IDs
        associated with your condition.\n\nmetric_description: A title for the metric
        to display in notifications.\n\nmetric: The metric to evaluate on.\n\nvalue_function:
        min, max, average, sample_size, total, percent\n\nrunbook_url: Runbook URL
        to display in notifications (optional).\n\nterms[duration] (in minutes): 5,
        10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any.\n\nplugin[id]: The ID of the plugin.\n\nplugin[guid]: The GUID of
        the plugin."
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
      description: "This API endpoint allows you to update Plugins conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        Alerts Plugins Conditions &gt; Create for an explanation of the field values
        ued in this command or the online document on\nupdating conditions for plugins."
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
      description: "This API endpoint allows you to delete Plugins conditions associated
        with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting Plugins conditions."
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
      description: "This API endpoint updates policy/channel associations.\n\nNote:
        Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
        on updating notification channels with policies."
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
    delete:
      summary: Delete Alerts Policy Channels. Format
      description: "This API endpoint deletes Alerts policy/channel associations.\n\nNote:
        Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
        on deleting notification channels with policies."
      operationId: deleteAlertsPolicyChannels.Format
      x-api-path-slug: alerts-policy-channels-format-delete
      parameters:
      - in: query
        name: channel_id
        description: Channel ID
        type: integer
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
  /alerts_channels.{format}:
    get:
      summary: Get Alerts Channels. Format
      description: |-
        This API endpoint works with new Alerts on alerts.newrelic.com.

        It returns a list of the channels associated with your New Relic account.

        See our documentation for a discussion on listing notification channels.
      operationId: getAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
    post:
      summary: Add Alerts Channels. Format
      description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
        creates a channel associated with your New Relic account.\n\nNote: Admin User\u2019s
        API Key is required.\n\nSee our documentation for a discussion on creating
        notification channels.\n\nChannel type configuration options:\n\n\n  \n    Email\n\n
        \   {\n\n    \"recipients\" : \"test@google.com\",\n\"include_json_attachment\"
        : true\n\n\n    }\n  \n  \n    HipChat\n\n    {\n\n    \"auth_token\": \"abc123\",\n\"room_id\":
        \"google.com\"\n\n\n    }\n  \n  \n    OpsGenie\n\n    {\n\n    \"api_key\":
        \"abc123\",\n\"teams\": \"team1\",\n\"tags\": \"tag1\",\n\"recipients\": \"me@me.com\"\n\n\n
        \   }\n  \n  \n    Slack\n\n    {\n\n    \"url\": \"http://test.com\",\n\"channel\":
        \"channel1\"\n\n\n    }\n  \n  \n    Campfire\n\n    {\n\n    \"subdomain\":
        \"mysubdomain\",\n\"token\": \"123abc\",\n\"room\": \"room1\"\n\n\n    }\n
        \ \n  \n    Victorops\n\n    {\n\n    \"key\": \"mykey\",\n\"route_key\":
        \"theroute\"\n\n\n    }\n  \n  \n    PagerDuty\n\n    {\n\n    \"service_key\":
        \"myservicekey\"\n\n\n    }\n  \n  \n    Webhook (json)\n\n    {\n\n    \"base_url\":
        \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/json\",\n\"payload\": {\"account_id\":
        1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\": \"test\",
        \"header2\": \"test\"}\n\n\n    }\n  \n  \n    Webhook (x-www-form-urlencoded)\n\n
        \   {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
        \"password\",\n\"payload_type\": \"application/x-www-form-urlencoded\",\n\"payload\":
        {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
        \"test\", \"header2\": \"test\"}\n\n\n    }"
      operationId: postAlertsChannels.Format
      x-api-path-slug: alerts-channels-format-post
      parameters:
      - in: body
        name: channel
        description: channel schema
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: policy_ids
        description: Policy IDs to associate with channel
        type: array
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels.
      - Format
  /alerts_channels/{channel_id}.{format}:
    delete:
      summary: Delete Alerts Channels Channel  . Format
      description: "This API endpoint deletes Alerts notification channels.\n\nNote:
        Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
        on deleting notification channels."
      operationId: deleteAlertsChannelsChannel.Format
      x-api-path-slug: alerts-channelschannel-id-format-delete
      parameters:
      - in: path
        name: channel_id
        description: Channel ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Channels
      - Channel
      - ""
      - .
      - Format
  /alerts_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create conditions for your alert
        policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
        for a discussion on creating conditions for policies.\n\n\nAll fields are
        required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults
        to false), \u201Cuser_defined\u201D.\n\ntype: apm_app_metric, apm_kt_metric,
        servers_metric, browser_metric, mobile_metric.\n\nname: A title for your condition.\n\nenabled:
        The status of your condition (optional).\n\nentities: An array of instance
        IDs associated with your condition.\n\nmetric: The metric field accepts parameters
        based on the condition type selected as follows:\n\n\_\_When apm_app_metric:
        apdex, error_percentage, response_time_web, response_time_background, throughput_web,
        throughput_background, user_defined.\n\n\_\_When apm_kt_metric: apdex, error_percentage,
        error_count, response_time, throughput.\n\n\_\_When servers_metric: cpu_percentage,
        disk_io_percentage, memory_percentage, fullest_disk_percentage, load_average_one_minute,
        user_defined.\n\n\_\_When browser_metric: end_user_apdex, total_page_load,
        page_rendering, web_application, network, dom_processing, request_queuing,
        ajax_response_time, page_views_with_js_errors, page_view_throughput, ajax_throughput,
        user_defined.\n\n\_\_When mobile_metric: database, images, json, network,
        view_loading, network_error_percentage, status_error_percentage, mobile_crash_rate,
        user_defined.\n\nrunbook_url: Runbook URL to display in notifications (optional).\n\nterms[duration]
        (in minutes): 5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any.\n\nuser_defined[metric]: A custom metric to be evaluated.\n\nuser_defined[value_function]:
        average, min, max, total, sample_size."
      operationId: postAlertsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-conditionspoliciespolicy-id-format-post
      parameters:
      - in: body
        name: condition
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
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_conditions/{id}.{format}:
    put:
      summary: Put Alerts Conditions  . Format
      description: "This API endpoint allows you to update conditions for your alert
        policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee Alerts Conditions
        &gt; Create for an explanation of the field values or the online \ndocumentation
        on updating conditions for policies."
      operationId: putAlertsConditions.Format
      x-api-path-slug: alerts-conditionsid-format-put
      parameters:
      - in: body
        name: condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Conditions
      - ""
      - .
      - Format
  /alerts_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Conditions Condition  . Format
      description: "This API endpoint allows you to delete conditions associated with
        your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting conditions."
      operationId: deleteAlertsConditionsCondition.Format
      x-api-path-slug: alerts-conditionscondition-id-format-delete
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
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_conditions.{format}:
    get:
      summary: Get Alerts Conditions. Format
      description: "This API endpoint allows you to list the conditions for your alert
        policy.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsConditions.Format
      x-api-path-slug: alerts-conditions-format-get
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
      - Conditions.
      - Format
  /alerts_entity_conditions/{entity_id}.{format}:
    get:
      summary: Get Alerts Entity Conditions Entity  . Format
      description: |-
        This API endpoint allows you to list the Alerts conditions an entity is part of.

        Entity type options (Synthetics is not yet supported):

        BrowserApplication

        Application

        MobileApplication

        Server

        KeyTransaction

        Plugin
      operationId: getAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-get
      parameters:
      - in: path
        name: entity_id
        description: Entity ID
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    put:
      summary: Put Alerts Entity Conditions Entity  . Format
      description: "This API endpoint allows you to add an entity to a specified Alerts
        condition.\n\nNote: Admin User\u2019s API Key is required.\n \n  Entity type
        options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
      operationId: putAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-put
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to add
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
    delete:
      summary: Delete Alerts Entity Conditions Entity  . Format
      description: "This API endpoint allows you to disassociate an entity with a
        specified Alerts condition.\n\nNote: Admin User\u2019s API Key is required.\n\nEntity
        type options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
      operationId: deleteAlertsEntityConditionsEntity.Format
      x-api-path-slug: alerts-entity-conditionsentity-id-format-delete
      parameters:
      - in: query
        name: condition_id
        description: Alerts condition ID
        type: integer
      - in: path
        name: entity_id
        description: Entity id to remove
        type: integer
      - in: query
        name: entity_type
        description: Entity Type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Entity
      - Conditions
      - Entity
      - ""
      - .
      - Format
  /alerts_events.{format}:
    get:
      summary: Get Alerts Events. Format
      description: "This API endpoint allows you to list the alert events for your
        account.\n\nAlerts events can be filter by product, target type, group ID,
        instance ID, and event type.\n\nThe options for products are: APM, BROWSER,
        MOBILE, SERVERS, PLUGINS, SYNTHETICS, and ALERTS.\n\nThe options for entity
        type are: Application, Server, KeyTransaction, Plugin, MobileApplication,
        BrowserApplication, and Monitor.\n\nThe options for event type are: NOTIFICATION,
        DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE, VIOLATION, and INSTRUMENTATION.\n\nThe
        group ID option is normally the same as the entity ID (e.g. an Application
        group ID and entity ID will be the same), however PLUGINS have a group ID
        representing the PLUGIN itself, and entity IDs for all instances of that PLUGIN
        type.\n\nSee our documentation for a discussion on \noutput pagination."
      operationId: getAlertsEvents.Format
      x-api-path-slug: alerts-events-format-get
      parameters:
      - in: query
        name: filter[entity_group_id]
        description: Filter by entity group ID
        type: integer
      - in: query
        name: filter[entity_id]
        description: Filter by entity ID
        type: integer
      - in: query
        name: filter[entity_type]
        description: Filter by entity type
        type: string
      - in: query
        name: filter[event_type]
        description: Filter by event type
        type: string
      - in: query
        name: filter[product]
        description: Filter by New Relic product
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Events.
      - Format
  /alerts_external_service_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts External Service Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create external service conditions
        for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating conditions for external services.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\ntype: apm_external_service, mobile_external_service.\n\nname:
        A title for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
        An array of instance IDs associated with your condition.\n\nexternal_service_url:
        The URL of the external service. Must not include protocol (\u201Cexample.com\u201D,
        not \u201Chttps://example.com\u201D)\n\nmetric: The metric field accepts parameters
        based on the condition type selected as follows:\n\n\_\_When apm_external_service:
        response_time_average, response_time_minimum, response_time_maximum, throughput.\n\n\_\_When
        mobile_external_service: response_time_average, response_time_minimum, response_time_maximum,
        throughput, network_failure_percentage, http_status_error_percentage.\n\nrunbook_url:
        Runbook URL to display in notifications (optional).\n\nterms[duration] (in
        minutes): 5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
        critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
        all, any."
      operationId: postAlertsExternalServiceConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-external-service-conditionspoliciespolicy-id-format-post
      parameters:
      - in: body
        name: external_service_condition
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
      - External
      - Service
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_external_service_conditions/{id}.{format}:
    put:
      summary: Put Alerts External Service Conditions  . Format
      description: "This API endpoint allows you to update external service conditions
        for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        Alerts External Service Conditions &gt; Create for an explanation of the field
        values used in this command or the online documentation on\nupdating conditions
        for external services."
      operationId: putAlertsExternalServiceConditions.Format
      x-api-path-slug: alerts-external-service-conditionsid-format-put
      parameters:
      - in: body
        name: external_service_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - External
      - Service
      - Conditions
      - ""
      - .
      - Format
  /alerts_external_service_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts External Service Conditions Condition  . Format
      description: "This API endpoint allows you to delete external service conditions
        associated with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting External services conditions."
      operationId: deleteAlertsExternalServiceConditionsCondition.Format
      x-api-path-slug: alerts-external-service-conditionscondition-id-format-delete
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
      - External
      - Service
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_external_service_conditions.{format}:
    get:
      summary: Get Alerts External Service Conditions. Format
      description: "This API endpoint allows you to list the external service conditions
        for your alert policy.\n\nSee our documentation for a discussion on \n output
        pagination."
      operationId: getAlertsExternalServiceConditions.Format
      x-api-path-slug: alerts-external-service-conditions-format-get
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
      - External
      - Service
      - Conditions.
      - Format
  /alerts_incidents.{format}:
    get:
      summary: Get Alerts Incents. Format
      description: "This API endpoint returns a list of the Incidents associated with
        your New Relic account.\n\nSee our documentation for a discussion on listing
        incidents \nand output pagination."
      operationId: getAlertsIncents.Format
      x-api-path-slug: alerts-incidents-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Incents.
      - Format
  /alerts_synthetics_conditions/policies/{policy_id}.{format}:
    post:
      summary: Add Alerts Synthetics Conditions Policies Policy  . Format
      description: "This API endpoint allows you to create Synthetics conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on creating Synthetic conditions.\n\nAll
        fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D
        (defaults to false).\n\nname: A title for your condition.\n\nmonitor_id: The
        GUID of the Synthetics monitor to alert on.\n\nrunbook_url: Runbook URL to
        display in notifications (optional).\n\nenabled: The status of your condition
        (optional)."
      operationId: postAlertsSyntheticsConditionsPoliciesPolicy.Format
      x-api-path-slug: alerts-synthetics-conditionspoliciespolicy-id-format-post
      parameters:
      - in: path
        name: policy_id
        description: Alerts policy ID
        type: integer
      - in: body
        name: synthetics_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions
      - Policies
      - Policy
      - ""
      - .
      - Format
  /alerts_synthetics_conditions/{id}.{format}:
    put:
      summary: Put Alerts Synthetics Conditions  . Format
      description: "This API endpoint allows you to update Synthetics conditions for
        your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on updating Synthetic conditions.\n\nSee
        Alerts Synthetics Conditions &gt; Create for an explanation of the field values
        used in this command."
      operationId: putAlertsSyntheticsConditions.Format
      x-api-path-slug: alerts-synthetics-conditionsid-format-put
      parameters:
      - in: path
        name: id
        description: Alerts condition ID to update
        type: integer
      - in: body
        name: synthetics_condition
        description: Condition schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Synthetics
      - Conditions
      - ""
      - .
      - Format
  /alerts_synthetics_conditions/{condition_id}.{format}:
    delete:
      summary: Delete Alerts Synthetics Conditions Condition  . Format
      description: "This API endpoint allows you to delete Synthetics conditions associated
        with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
        our documentation for a discussion on deleting Synthetic conditions."
      operationId: deleteAlertsSyntheticsConditionsCondition.Format
      x-api-path-slug: alerts-synthetics-conditionscondition-id-format-delete
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
      - Synthetics
      - Conditions
      - Condition
      - ""
      - .
      - Format
  /alerts_synthetics_conditions.{format}:
    get:
      summary: Get Alerts Synthetics Conditions. Format
      description: |-
        This API endpoint allows you to list the Synthetics conditions for your alert policy.

        See our documentation for a discussion on listing Synthetic conditions
        and  output pagination.
      operationId: getAlertsSyntheticsConditions.Format
      x-api-path-slug: alerts-synthetics-conditions-format-get
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
      - Synthetics
      - Conditions.
      - Format
  /alerts_violations.{format}:
    get:
      summary: Get Alerts Violations. Format
      description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
        returns a list of the violations associated with your New Relic account.\n\nSee
        our documentation for a discussion on \noutput pagination."
      operationId: getAlertsViolations.Format
      x-api-path-slug: alerts-violations-format-get
      parameters:
      - in: query
        name: only_open
        description: Filter by open violations
        type: boolean
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Violations.
      - Format
  /applications/{application_id}/deployments.{format}:
    get:
      summary: Get Applications Application  Deployments. Format
      description: |-
        This API endpoint returns a paginated list of the deployments associated with a given application.

        See our documentation for a discussion on output pagination.
      operationId: getApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeployments-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments.
      - Format
    post:
      summary: Add Applications Application  Deployments. Format
      description: "This API endpoint creates a deployment record for a given application.\nDeployment
        records are created with the following attributes:\n\nRequired:\n\_\_- Application
        ID\n\_\_- Revision, such as a git SHA\n\nOptional:\n\_\_- Changelog \n\_\_-
        Description \n\_\_- User posting the deployment\n\nNote that the time of your
        deployment will be recorded as the current time in UTC."
      operationId: postApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeployments-format-post
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: body
        name: deployment
        description: Deployment schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments.
      - Format
  /applications/{application_id}/deployments/{id}.{format}:
    delete:
      summary: Delete Applications Application  Deployments  . Format
      description: "This API endpoint deletes the specified deployment record.\n\nNote:
        Admin User\u2019s API Key is required."
      operationId: deleteApplicationsApplicationDeployments.Format
      x-api-path-slug: applicationsapplication-iddeploymentsid-format-delete
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: path
        name: id
        description: Deployment ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Deployments
      - ""
      - .
      - Format
  /applications/{application_id}/hosts.{format}:
    get:
      summary: Get Applications Application  Hosts. Format
      description: "This API endpoint returns a \npaginated list of hosts associated
        with the given application. The time range for summary data is the last 10
        minutes.\n\nApplication hosts can be filtered by hostname, or the list of
        application host IDs.\n\nSee our documentation for a discussion and examples
        of\nusing  filters \nand summary data output."
      operationId: getApplicationsApplicationHosts.Format
      x-api-path-slug: applicationsapplication-idhosts-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: filter[hostname]
        description: Filter by server hostname
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application host ids
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Hosts.
      - Format
  /applications/{application_id}/hosts/{id}.{format}:
    get:
      summary: Get Applications Application  Hosts  . Format
      description: |-
        This API endpoint returns a single application host, identified by ID. The time range for summary data is the last 10 minutes.

        See our documentation for a discussion of
        summary data output.
      operationId: getApplicationsApplicationHosts.Format
      x-api-path-slug: applicationsapplication-idhostsid-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: path
        name: id
        description: Application host ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Hosts
      - ""
      - .
      - Format
  /applications/{application_id}/hosts/{host_id}/metrics.{format}:
    get:
      summary: Get Applications Application  Hosts Host  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getApplicationsApplicationHostsHostMetrics.Format
      x-api-path-slug: applicationsapplication-idhostshost-idmetrics-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: path
        name: host_id
        description: Application Host ID
        type: integer
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Hosts
      - Host
      - ""
      - Metrics.
      - Format
  /applications/{application_id}/hosts/{host_id}/metrics/data.{format}:
    get:
      summary: Get Applications Application  Hosts Host  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getApplicationsApplicationHostsHostMetricsData.Format
      x-api-path-slug: applicationsapplication-idhostshost-idmetricsdata-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: path
        name: host_id
        description: Application Host ID
        type: integer
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Hosts
      - Host
      - ""
      - Metrics
      - Data.
      - Format
  /applications/{application_id}/instances.{format}:
    get:
      summary: Get Applications Application  Instances. Format
      description: "This API endpoint returns a \npaginated list of instances associated
        with the given application. The time range for summary data is the last 10
        minutes.\n\nApplication instances can be filtered by hostname, or the list
        of application instance IDs.\n\nSee our documentation for a discussion and
        examples of\nusing  filters \nand summary data output."
      operationId: getApplicationsApplicationInstances.Format
      x-api-path-slug: applicationsapplication-idinstances-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: filter[hostname]
        description: Filter by server hostname
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application instance ids
        type: list
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances.
      - Format
  /applications/{application_id}/instances/{id}.{format}:
    get:
      summary: Get Applications Application  Instances  . Format
      description: |-
        This API endpoint returns a single application instance, identified by ID. The time range for summary data is the last 10 minutes.

        See our documentation for a discussion of
         summary data output.
      operationId: getApplicationsApplicationInstances.Format
      x-api-path-slug: applicationsapplication-idinstancesid-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: path
        name: id
        description: Application instance ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - ""
      - .
      - Format
  /applications/{application_id}/instances/{instance_id}/metrics.{format}:
    get:
      summary: Get Applications Application  Instances Instance  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getApplicationsApplicationInstancesInstanceMetrics.Format
      x-api-path-slug: applicationsapplication-idinstancesinstance-idmetrics-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: path
        name: instance_id
        description: Application Instance ID
        type: integer
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - Instance
      - ""
      - Metrics.
      - Format
  /applications/{application_id}/instances/{instance_id}/metrics/data.{format}:
    get:
      summary: Get Applications Application  Instances Instance  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getApplicationsApplicationInstancesInstanceMetricsData.Format
      x-api-path-slug: applicationsapplication-idinstancesinstance-idmetricsdata-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: path
        name: instance_id
        description: Application Instance ID
        type: integer
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Instances
      - Instance
      - ""
      - Metrics
      - Data.
      - Format
  /applications.{format}:
    get:
      summary: Get Applications. Format
      description: "This API endpoint returns a paginated\nlist of the Applications
        associated with your New Relic account. The time range for summary data is
        the last 10 minutes.\n\nApplications can be filtered by their name, hosts,
        the list of application IDs or the application language as\nreported by the
        agents.\n\nSee our documentation for a discussion and examples of\nusing  filters
        \nand summary data output."
      operationId: getApplications.Format
      x-api-path-slug: applications-format-get
      parameters:
      - in: query
        name: filter[host]
        description: Filter by application host
        type: string
      - in: query
        name: filter[ids]
        description: Filter by application ids
        type: list
      - in: query
        name: filter[language]
        description: Filter by application language
        type: string
      - in: query
        name: filter[name]
        description: Filter by application name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications.
      - Format
  /applications/{id}.{format}:
    get:
      summary: Get Applications  . Format
      description: |-
        This API endpoint returns a single Application, identified by ID. The time range for summary data is the last 10 minutes.

        See our documentation for a discussion of the
         summary data output.
      operationId: getApplications.Format
      x-api-path-slug: applicationsid-format-get
      parameters:
      - in: path
        name: id
        description: Application ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - ""
      - .
      - Format
    put:
      summary: Put Applications  . Format
      description: |-
        This API endpoint allows you to update certain parameters of your application.

        The input is expected to be in JSON or XML format in the body parameter of the PUT request. The exact
        schema is defined below. Any extra parameters passed in the body will be ignored.

        See our documentation for a discussion and simple example of
         updating
        an application.
      operationId: putApplications.Format
      x-api-path-slug: applicationsid-format-put
      parameters:
      - in: body
        name: application
        description: Application schema
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Application ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - ""
      - .
      - Format
    delete:
      summary: Delete Applications  . Format
      description: |-
        This API endpoint deletes an application and all of its reported data.

        WARNING: Only applications that have stopped reporting can be deleted. This is an irreversible process
        which will delete all reported data for this application.
      operationId: deleteApplications.Format
      x-api-path-slug: applicationsid-format-delete
      parameters:
      - in: path
        name: id
        description: Application ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - ""
      - .
      - Format
  /applications/{application_id}/metrics.{format}:
    get:
      summary: Get Applications Application  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getApplicationsApplicationMetrics.Format
      x-api-path-slug: applicationsapplication-idmetrics-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Metrics.
      - Format
  /applications/{application_id}/metrics/data.{format}:
    get:
      summary: Get Applications Application  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getApplicationsApplicationMetricsData.Format
      x-api-path-slug: applicationsapplication-idmetricsdata-format-get
      parameters:
      - in: path
        name: application_id
        description: Application ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Applications
      - Application
      - ""
      - Metrics
      - Data.
      - Format
  /browser_applications.{format}:
    get:
      summary: Get Browser Applications. Format
      description: |-
        This API endpoint returns a list of the Browser Applications associated with your New Relic account.

        Browser Applications can be filtered by their name, or by the application IDs.
      operationId: getBrowserApplications.Format
      x-api-path-slug: browser-applications-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by application ids
        type: list
      - in: query
        name: filter[name]
        description: Filter by application name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Applications.
      - Format
    post:
      summary: Add Browser Applications. Format
      description: This API endpoint allows you to create a standalone Browser Application.
      operationId: postBrowserApplications.Format
      x-api-path-slug: browser-applications-format-post
      parameters:
      - in: body
        name: browser_application
        description: Browser Application Schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Browser
      - Applications.
      - Format
  /components.{format}:
    get:
      summary: Get Components. Format
      description: |-
        This API endpoint returns a list of the plugin components associated with your New Relic account.

        Plugins can be filtered by their name, the list of component IDs or a plugin ID.

        See our documentation for a discussion on  listing components
        and  output pagination.
      operationId: getComponents.Format
      x-api-path-slug: components-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter components by ids
        type: list
      - in: query
        name: filter[name]
        description: Filter components by name
        type: string
      - in: query
        name: filter[plugin_id]
        description: Filter components by the plugin
        type: integer
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components.
      - Format
  /components/{id}.{format}:
    get:
      summary: Get Components  . Format
      description: |-
        This API endpoint returns a single component, identified by its ID.

        See our documentation for a discussion on listing components by ID.
      operationId: getComponents.Format
      x-api-path-slug: componentsid-format-get
      parameters:
      - in: path
        name: id
        description: Plugin ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components
      - ""
      - .
      - Format
  /components/{component_id}/metrics.{format}:
    get:
      summary: Get Components Component  Metrics. Format
      description: |-
        Return a list of known metrics and their value names for the given resource.

        See our documentation for a discussion
        on  output pagination
        and for examples of requesting and using metric values.
      operationId: getComponentsComponentMetrics.Format
      x-api-path-slug: componentscomponent-idmetrics-format-get
      parameters:
      - in: path
        name: component_id
        description: Component ID
        type: integer
      - in: query
        name: cursor
        description: Cursor for next page (replacing page param)
        type: string
      - in: query
        name: name
        description: Filter metrics by name
        type: string
      - in: query
        name: page
        description: Pagination index (will be deprecated)
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Components
      - Component
      - ""
      - Metrics.
      - Format
  /components/{component_id}/metrics/data.{format}:
    get:
      summary: Get Components Component  Metrics Data. Format
      description: "This API endpoint returns a list of values for each of the requested
        metrics. The list of available metrics\ncan be returned using the Metric Name
        API endpoint.\n\nMetric data can be filtered by a number of parameters, including
        multiple names and values, and by time range.\nMetric names and values will
        be matched intelligently in the background.\n\nYou can also retrieve a summarized
        data point across the entire time range selected by using the summarize\nparameter.\n\nSee
        our documentation for a discussion on \noutput pagination,  time range \nrelated
        considerations, and for examples of requesting and using metric values."
      operationId: getComponentsComponentMetricsData.Format
      x-api-path-slug: componentscomponent-idmetricsdata-format-get
      parameters:
      - in: path
        name: component_id
        description: Component ID
        type: integer
      - in: query
        name: from
        description: Retrieve metrics after this time
        type: time
      - in: query
        name: names
        description: Retrieve specific metrics by name
        type: array
      - in: query
        name: period
        description: Period of timeslices in seconds
        type: integer
      - in: query
        name: raw
        description: Return unformatted raw values
        type: boolean
      - in: query
        name: summarize
        description: Summarize the data
        type: boolean
      - in: query
        name: to
        description: Retrieve metrics before this time
        type: time
      - in: query
        name: values
        description: Retrieve specific metric values
        type: array
      responses:
        200:
          description: OK
      tags:
      - Components
      - Component
      - ""
      - Metrics
      - Data.
      - Format
  /key_transactions.{format}:
    get:
      summary: Get Key Transactions. Format
      description: "This API endpoint returns a paginated \nlist of the key transactions
        associated with your New Relic account.  The time range for summary data is
        the last 10 minutes.\n\nKey transactions can be filtered by their name or
        list of IDs.\n\nSee our documentation for a discussion of \nsummary data output."
      operationId: getKeyTransactions.Format
      x-api-path-slug: key-transactions-format-get
      parameters:
      - in: query
        name: filter[ids]
        description: Filter by policy IDs
        type: list
      - in: query
        name: filter[name]
        description: Filter by name
        type: string
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Key
      - Transactions.
      - Format
  /key_transactions/{id}.{format}:
    get:
      summary: Get Key Transactions  . Format
      description: "This endpoint returns a single key transaction, identified by
        ID. The time range for summary data is the last 10 minutes.\n\nSee our documentation
        for a discussion of \nsummary data output."
      operationId: getKeyTransactions.Format
      x-api-path-slug: key-transactionsid-format-get
      parameters:
      - in: path
        name: id
        description: Key transaction ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Key
      - Transactions
      - ""
      - .
      - Format
  /labels.{format}:
    get:
      summary: Get Labels. Format
      description: This API endpoint returns a paginated list of the labels available
        for the account.
      operationId: getLabels.Format
      x-api-path-slug: labels-format-get
      parameters:
      - in: query
        name: page
        description: Pagination index
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Labels.
      - Format
    put:
      summary: Put Labels. Format
      description: "This API endpoint will create a new label with the provided category
        and name.\n\nInclude the application and server IDs to which the label should
        be applied in the corresponding arrays.\nYou may omit the \u201Clinks\u201D
        or \u201Cservers\u201D arrays, if not needed.\n\nSee our documentation for
        a discussion on obtaining \napplication \nand \nserver IDs."
      operationId: putLabels.Format
      x-api-path-slug: labels-format-put
      parameters:
      - in: body
        name: label
        description: Label schema
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Labels.
      - Format
  /labels/{key}.{format}:
    delete:
      summary: Delete Labels Key . Format
      description: |-
        When applications are provided, this endpoint will remove those applications from the label.

        When no applications are provided, this endpoint will remove the label.
      operationId: deleteLabelsKey.Format
      x-api-path-slug: labelskey-format-delete
      parameters:
      - in: path
        name: key
        description: Label key
        type: string
      responses:
        200:
          description: OK
      tags:
      - Labels
      - Key
      - .
      - Format
  /mobile_applications.{format}:
    get:
      summary: Get Mobile Applications. Format
      description: |-
        This API endpoint returns a list of the Mobile Applications associated with your New Relic account.

        MobileApplications can be filtered by their name, or by the application IDs.
      operationId: getMobileApplications.Format
      x-api-path-slug: mobile-applications-format-get
      responses:
        200:
          description: OK
      tags:
      - Mobile
      - Applications.
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