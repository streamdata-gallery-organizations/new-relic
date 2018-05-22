---
name: New Relic
x-slug: new-relic
description: "New Relic\u2019s digital intelligence platform lets developers, ops,
  and tech teams measure and monitor the performance of their applications and infrastructure."
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: New Relic
created: "2018-05-22"
modified: "2018-05-22"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Add Alerts Plugins Conditions Policies Policy  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to create Plugins conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
    for a discussion on creating conditions for plugins.\n\nAll fields are required
    except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults to false).\n\nname:
    A title for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
    An array of instance IDs associated with your condition.\n\nmetric_description:
    A title for the metric to display in notifications.\n\nmetric: The metric to evaluate
    on.\n\nvalue_function: min, max, average, sample_size, total, percent\n\nrunbook_url:
    Runbook URL to display in notifications (optional).\n\nterms[duration] (in minutes):
    5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
    critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
    all, any.\n\nplugin[id]: The ID of the plugin.\n\nplugin[guid]: The GUID of the
    plugin."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/policies/{policy_id}.{format}
  tags: Alerts, Plugins, Conditions, Policies, Policy, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-plugins-conditionspoliciespolicy-idformat-post-openapi.md
- name: New Relic Put Alerts Plugins Conditions  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to update Plugins conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee Alerts
    Plugins Conditions &gt; Create for an explanation of the field values ued in this
    command or the online document on\nupdating conditions for plugins."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/{id}.{format}
  tags: Alerts, Plugins, Conditions, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-plugins-conditionsidformat-put-openapi.md
- name: New Relic Delete Alerts Plugins Conditions Condition  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to delete Plugins conditions associated
    with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    our documentation for a discussion on deleting Plugins conditions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/{condition_id}.{format}
  tags: Alerts, Plugins, Conditions, Condition, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-plugins-conditionscondition-idformat-delete-openapi.md
- name: New Relic Get Alerts Plugins Conditions. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the Plugins conditions for your
    alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions.{format}
  tags: Alerts, Plugins, Conditions., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-plugins-conditionsformat-get-openapi.md
- name: New Relic Put Alerts Policy Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint updates policy/channel associations.\n\nNote: Admin
    User\u2019s API Key is required.\n\nSee our documentation for a discussion on
    updating notification channels with policies."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_policy_channels.{format}
  tags: Alerts, Policy, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-policy-channelsformat-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-policy-channelsformat-put-openapi.md
- name: New Relic Delete Alerts Policy Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint deletes Alerts policy/channel associations.\n\nNote:
    Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
    on deleting notification channels with policies."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_policy_channels.{format}
  tags: Alerts, Policy, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-policy-channelsformat-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-policy-channelsformat-delete-openapi.md
- name: New Relic Get Alerts Channels. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint works with new Alerts on alerts.newrelic.com.

    It returns a list of the channels associated with your New Relic account.

    See our documentation for a discussion on listing notification channels.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels.{format}
  tags: Alerts, Channels., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-channelsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-channelsformat-get-openapi.md
- name: New Relic Add Alerts Channels. Format
  x-api-slug: new-relic
  description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
    creates a channel associated with your New Relic account.\n\nNote: Admin User\u2019s
    API Key is required.\n\nSee our documentation for a discussion on creating notification
    channels.\n\nChannel type configuration options:\n\n\n  \n    Email\n\n    {\n\n
    \   \"recipients\" : \"test@google.com\",\n\"include_json_attachment\" : true\n\n\n
    \   }\n  \n  \n    HipChat\n\n    {\n\n    \"auth_token\": \"abc123\",\n\"room_id\":
    \"google.com\"\n\n\n    }\n  \n  \n    OpsGenie\n\n    {\n\n    \"api_key\": \"abc123\",\n\"teams\":
    \"team1\",\n\"tags\": \"tag1\",\n\"recipients\": \"me@me.com\"\n\n\n    }\n  \n
    \ \n    Slack\n\n    {\n\n    \"url\": \"http://test.com\",\n\"channel\": \"channel1\"\n\n\n
    \   }\n  \n  \n    Campfire\n\n    {\n\n    \"subdomain\": \"mysubdomain\",\n\"token\":
    \"123abc\",\n\"room\": \"room1\"\n\n\n    }\n  \n  \n    Victorops\n\n    {\n\n
    \   \"key\": \"mykey\",\n\"route_key\": \"theroute\"\n\n\n    }\n  \n  \n    PagerDuty\n\n
    \   {\n\n    \"service_key\": \"myservicekey\"\n\n\n    }\n  \n  \n    Webhook
    (json)\n\n    {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\":
    \"username\",\n\"auth_password\": \"password\",\n\"payload_type\": \"application/json\",\n\"payload\":
    {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
    \"test\", \"header2\": \"test\"}\n\n\n    }\n  \n  \n    Webhook (x-www-form-urlencoded)\n\n
    \   {\n\n    \"base_url\": \"http://test.com\",\n\"auth_username\": \"username\",\n\"auth_password\":
    \"password\",\n\"payload_type\": \"application/x-www-form-urlencoded\",\n\"payload\":
    {\"account_id\": 1, \"account_name\": \"account name\" },\n\"headers\": {\"header1\":
    \"test\", \"header2\": \"test\"}\n\n\n    }"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels.{format}
  tags: Alerts, Channels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-channelsformat-post-openapi.md
- name: New Relic Delete Alerts Channels Channel  . Format
  x-api-slug: new-relic
  description: "This API endpoint deletes Alerts notification channels.\n\nNote: Admin
    User\u2019s API Key is required.\n\nSee our documentation for a discussion on
    deleting notification channels."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_channels/{channel_id}.{format}
  tags: Alerts, Channels, Channel, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-channelschannel-idformat-delete-openapi.md
- name: New Relic Add Alerts Conditions Policies Policy  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to create conditions for your alert policies.\n\nNote:
    Admin User\u2019s API Key is required.\n\nSee our documentation for a discussion
    on creating conditions for policies.\n\n\nAll fields are required except for \u201Crunbook_url\u201D,
    \u201Cenabled\u201D (defaults to false), \u201Cuser_defined\u201D.\n\ntype: apm_app_metric,
    apm_kt_metric, servers_metric, browser_metric, mobile_metric.\n\nname: A title
    for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
    An array of instance IDs associated with your condition.\n\nmetric: The metric
    field accepts parameters based on the condition type selected as follows:\n\n\_\_When
    apm_app_metric: apdex, error_percentage, response_time_web, response_time_background,
    throughput_web, throughput_background, user_defined.\n\n\_\_When apm_kt_metric:
    apdex, error_percentage, error_count, response_time, throughput.\n\n\_\_When servers_metric:
    cpu_percentage, disk_io_percentage, memory_percentage, fullest_disk_percentage,
    load_average_one_minute, user_defined.\n\n\_\_When browser_metric: end_user_apdex,
    total_page_load, page_rendering, web_application, network, dom_processing, request_queuing,
    ajax_response_time, page_views_with_js_errors, page_view_throughput, ajax_throughput,
    user_defined.\n\n\_\_When mobile_metric: database, images, json, network, view_loading,
    network_error_percentage, status_error_percentage, mobile_crash_rate, user_defined.\n\nrunbook_url:
    Runbook URL to display in notifications (optional).\n\nterms[duration] (in minutes):
    5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
    critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
    all, any.\n\nuser_defined[metric]: A custom metric to be evaluated.\n\nuser_defined[value_function]:
    average, min, max, total, sample_size."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_conditions/policies/{policy_id}.{format}
  tags: Alerts, Conditions, Policies, Policy, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-conditionspoliciespolicy-idformat-post-openapi.md
- name: New Relic Put Alerts Conditions  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to update conditions for your alert policies.\n\nNote:
    Admin User\u2019s API Key is required.\n\nSee Alerts Conditions &gt; Create for
    an explanation of the field values or the online \ndocumentation on updating conditions
    for policies."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_conditions/{id}.{format}
  tags: Alerts, Conditions, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-conditionsidformat-put-openapi.md
- name: New Relic Delete Alerts Conditions Condition  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to delete conditions associated with
    your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our
    documentation for a discussion on deleting conditions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_conditions/{condition_id}.{format}
  tags: Alerts, Conditions, Condition, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-conditionscondition-idformat-delete-openapi.md
- name: New Relic Get Alerts Conditions. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the conditions for your alert
    policy.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_conditions.{format}
  tags: Alerts, Conditions., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-conditionsformat-get-openapi.md
- name: New Relic Get Alerts Entity Conditions Entity  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint allows you to list the Alerts conditions an entity is part of.

    Entity type options (Synthetics is not yet supported):

    BrowserApplication

    Application

    MobileApplication

    Server

    KeyTransaction

    Plugin
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_entity_conditions/{entity_id}.{format}
  tags: Alerts, Entity, Conditions, Entity, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-entity-conditionsentity-idformat-get-openapi.md
- name: New Relic Put Alerts Entity Conditions Entity  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to add an entity to a specified Alerts
    condition.\n\nNote: Admin User\u2019s API Key is required.\n \n  Entity type options
    (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_entity_conditions/{entity_id}.{format}
  tags: Alerts, Entity, Conditions, Entity, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-entity-conditionsentity-idformat-put-openapi.md
- name: New Relic Delete Alerts Entity Conditions Entity  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to disassociate an entity with a specified
    Alerts condition.\n\nNote: Admin User\u2019s API Key is required.\n\nEntity type
    options (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_entity_conditions/{entity_id}.{format}
  tags: Alerts, Entity, Conditions, Entity, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-entity-conditionsentity-idformat-delete-openapi.md
- name: New Relic Get Alerts Events. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the alert events for your account.\n\nAlerts
    events can be filter by product, target type, group ID, instance ID, and event
    type.\n\nThe options for products are: APM, BROWSER, MOBILE, SERVERS, PLUGINS,
    SYNTHETICS, and ALERTS.\n\nThe options for entity type are: Application, Server,
    KeyTransaction, Plugin, MobileApplication, BrowserApplication, and Monitor.\n\nThe
    options for event type are: NOTIFICATION, DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE,
    VIOLATION, and INSTRUMENTATION.\n\nThe group ID option is normally the same as
    the entity ID (e.g. an Application group ID and entity ID will be the same), however
    PLUGINS have a group ID representing the PLUGIN itself, and entity IDs for all
    instances of that PLUGIN type.\n\nSee our documentation for a discussion on \noutput
    pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_events.{format}
  tags: Alerts, Events., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-eventsformat-get-openapi.md
- name: New Relic Add Alerts External Service Conditions Policies Policy  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to create external service conditions
    for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    our documentation for a discussion on creating conditions for external services.\n\nAll
    fields are required except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults
    to false).\n\ntype: apm_external_service, mobile_external_service.\n\nname: A
    title for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
    An array of instance IDs associated with your condition.\n\nexternal_service_url:
    The URL of the external service. Must not include protocol (\u201Cexample.com\u201D,
    not \u201Chttps://example.com\u201D)\n\nmetric: The metric field accepts parameters
    based on the condition type selected as follows:\n\n\_\_When apm_external_service:
    response_time_average, response_time_minimum, response_time_maximum, throughput.\n\n\_\_When
    mobile_external_service: response_time_average, response_time_minimum, response_time_maximum,
    throughput, network_failure_percentage, http_status_error_percentage.\n\nrunbook_url:
    Runbook URL to display in notifications (optional).\n\nterms[duration] (in minutes):
    5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
    critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
    all, any."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_external_service_conditions/policies/{policy_id}.{format}
  tags: Alerts, External, Service, Conditions, Policies, Policy, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-external-service-conditionspoliciespolicy-idformat-post-openapi.md
- name: New Relic Put Alerts External Service Conditions  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to update external service conditions
    for your alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    Alerts External Service Conditions &gt; Create for an explanation of the field
    values used in this command or the online documentation on\nupdating conditions
    for external services."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_external_service_conditions/{id}.{format}
  tags: Alerts, External, Service, Conditions, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-external-service-conditionsidformat-put-openapi.md
- name: New Relic Delete Alerts External Service Conditions Condition  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to delete external service conditions
    associated with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    our documentation for a discussion on deleting External services conditions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_external_service_conditions/{condition_id}.{format}
  tags: Alerts, External, Service, Conditions, Condition, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-external-service-conditionscondition-idformat-delete-openapi.md
- name: New Relic Get Alerts External Service Conditions. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the external service conditions
    for your alert policy.\n\nSee our documentation for a discussion on \n output
    pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_external_service_conditions.{format}
  tags: Alerts, External, Service, Conditions., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-external-service-conditionsformat-get-openapi.md
- name: New Relic Get Alerts Incents. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of the Incidents associated with
    your New Relic account.\n\nSee our documentation for a discussion on listing incidents
    \nand output pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_incidents.{format}
  tags: Alerts, Incents., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-incidentsformat-get-openapi.md
- name: New Relic Add Alerts Synthetics Conditions Policies Policy  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to create Synthetics conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
    for a discussion on creating Synthetic conditions.\n\nAll fields are required
    except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults to false).\n\nname:
    A title for your condition.\n\nmonitor_id: The GUID of the Synthetics monitor
    to alert on.\n\nrunbook_url: Runbook URL to display in notifications (optional).\n\nenabled:
    The status of your condition (optional)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_synthetics_conditions/policies/{policy_id}.{format}
  tags: Alerts, Synthetics, Conditions, Policies, Policy, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-synthetics-conditionspoliciespolicy-idformat-post-openapi.md
- name: New Relic Put Alerts Synthetics Conditions  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to update Synthetics conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
    for a discussion on updating Synthetic conditions.\n\nSee Alerts Synthetics Conditions
    &gt; Create for an explanation of the field values used in this command."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_synthetics_conditions/{id}.{format}
  tags: Alerts, Synthetics, Conditions, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-synthetics-conditionsidformat-put-openapi.md
- name: New Relic Delete Alerts Synthetics Conditions Condition  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to delete Synthetics conditions associated
    with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    our documentation for a discussion on deleting Synthetic conditions."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_synthetics_conditions/{condition_id}.{format}
  tags: Alerts, Synthetics, Conditions, Condition, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-synthetics-conditionscondition-idformat-delete-openapi.md
- name: New Relic Get Alerts Synthetics Conditions. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint allows you to list the Synthetics conditions for your alert policy.

    See our documentation for a discussion on listing Synthetic conditions
    and  output pagination.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_synthetics_conditions.{format}
  tags: Alerts, Synthetics, Conditions., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-synthetics-conditionsformat-get-openapi.md
- name: New Relic Get Alerts Violations. Format
  x-api-slug: new-relic
  description: "This API endpoint works with new Alerts on alerts.newrelic.com.\n\nIt
    returns a list of the violations associated with your New Relic account.\n\nSee
    our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_violations.{format}
  tags: Alerts, Violations., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/alerts-violationsformat-get-openapi.md
- name: New Relic Get Applications Application  Deployments. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a paginated list of the deployments associated with a given application.

    See our documentation for a discussion on output pagination.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/deployments.{format}
  tags: Applications, Application, , Deployments., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-iddeploymentsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-iddeploymentsformat-get-openapi.md
- name: New Relic Add Applications Application  Deployments. Format
  x-api-slug: new-relic
  description: "This API endpoint creates a deployment record for a given application.\nDeployment
    records are created with the following attributes:\n\nRequired:\n\_\_- Application
    ID\n\_\_- Revision, such as a git SHA\n\nOptional:\n\_\_- Changelog \n\_\_- Description
    \n\_\_- User posting the deployment\n\nNote that the time of your deployment will
    be recorded as the current time in UTC."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/deployments.{format}
  tags: Applications, Application, , Deployments., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-iddeploymentsformat-post-openapi.md
- name: New Relic Delete Applications Application  Deployments  . Format
  x-api-slug: new-relic
  description: "This API endpoint deletes the specified deployment record.\n\nNote:
    Admin User\u2019s API Key is required."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/deployments/{id}.{format}
  tags: Applications, Application, , Deployments, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-iddeploymentsidformat-delete-openapi.md
- name: New Relic Get Applications Application  Hosts. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a \npaginated list of hosts associated with
    the given application. The time range for summary data is the last 10 minutes.\n\nApplication
    hosts can be filtered by hostname, or the list of application host IDs.\n\nSee
    our documentation for a discussion and examples of\nusing  filters \nand summary
    data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/hosts.{format}
  tags: Applications, Application, , Hosts., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idhostsformat-get-openapi.md
- name: New Relic Get Applications Application  Hosts  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a single application host, identified by ID. The time range for summary data is the last 10 minutes.

    See our documentation for a discussion of
    summary data output.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/hosts/{id}.{format}
  tags: Applications, Application, , Hosts, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idhostsidformat-get-openapi.md
- name: New Relic Get Applications Application  Hosts Host  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/hosts/{host_id}/metrics.{format}
  tags: Applications, Application, , Hosts, Host, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idhostshost-idmetricsformat-get-openapi.md
- name: New Relic Get Applications Application  Hosts Host  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/hosts/{host_id}/metrics/data.{format}
  tags: Applications, Application, , Hosts, Host, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idhostshost-idmetricsdataformat-get-openapi.md
- name: New Relic Get Applications Application  Instances. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a \npaginated list of instances associated
    with the given application. The time range for summary data is the last 10 minutes.\n\nApplication
    instances can be filtered by hostname, or the list of application instance IDs.\n\nSee
    our documentation for a discussion and examples of\nusing  filters \nand summary
    data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/instances.{format}
  tags: Applications, Application, , Instances., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idinstancesformat-get-openapi.md
- name: New Relic Get Applications Application  Instances  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a single application instance, identified by ID. The time range for summary data is the last 10 minutes.

    See our documentation for a discussion of
     summary data output.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/instances/{id}.{format}
  tags: Applications, Application, , Instances, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idinstancesidformat-get-openapi.md
- name: New Relic Get Applications Application  Instances Instance  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/instances/{instance_id}/metrics.{format}
  tags: Applications, Application, , Instances, Instance, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idinstancesinstance-idmetricsformat-get-openapi.md
- name: New Relic Get Applications Application  Instances Instance  Metrics Data.
    Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/instances/{instance_id}/metrics/data.{format}
  tags: Applications, Application, , Instances, Instance, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idinstancesinstance-idmetricsdataformat-get-openapi.md
- name: New Relic Get Applications. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a paginated\nlist of the Applications associated
    with your New Relic account. The time range for summary data is the last 10 minutes.\n\nApplications
    can be filtered by their name, hosts, the list of application IDs or the application
    language as\nreported by the agents.\n\nSee our documentation for a discussion
    and examples of\nusing  filters \nand summary data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications.{format}
  tags: Applications., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsformat-get-openapi.md
- name: New Relic Get Applications  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a single Application, identified by ID. The time range for summary data is the last 10 minutes.

    See our documentation for a discussion of the
     summary data output.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{id}.{format}
  tags: Applications, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsidformat-get-openapi.md
- name: New Relic Put Applications  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint allows you to update certain parameters of your application.

    The input is expected to be in JSON or XML format in the body parameter of the PUT request. The exact
    schema is defined below. Any extra parameters passed in the body will be ignored.

    See our documentation for a discussion and simple example of
     updating
    an application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{id}.{format}
  tags: Applications, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsidformat-put-openapi.md
- name: New Relic Delete Applications  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint deletes an application and all of its reported data.

    WARNING: Only applications that have stopped reporting can be deleted. This is an irreversible process
    which will delete all reported data for this application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{id}.{format}
  tags: Applications, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsidformat-delete-openapi.md
- name: New Relic Get Applications Application  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/metrics.{format}
  tags: Applications, Application, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idmetricsformat-get-openapi.md
- name: New Relic Get Applications Application  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///applications/{application_id}/metrics/data.{format}
  tags: Applications, Application, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/applicationsapplication-idmetricsdataformat-get-openapi.md
- name: New Relic Get Browser Applications. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a list of the Browser Applications associated with your New Relic account.

    Browser Applications can be filtered by their name, or by the application IDs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///browser_applications.{format}
  tags: Browser, Applications., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/browser-applicationsformat-get-openapi.md
- name: New Relic Add Browser Applications. Format
  x-api-slug: new-relic
  description: This API endpoint allows you to create a standalone Browser Application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///browser_applications.{format}
  tags: Browser, Applications., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/browser-applicationsformat-post-openapi.md
- name: New Relic Get Components. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a list of the plugin components associated with your New Relic account.

    Plugins can be filtered by their name, the list of component IDs or a plugin ID.

    See our documentation for a discussion on  listing components
    and  output pagination.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components.{format}
  tags: Components., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentsformat-get-openapi.md
- name: New Relic Get Components  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a single component, identified by its ID.

    See our documentation for a discussion on listing components by ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{id}.{format}
  tags: Components, , ., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentsidformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentsidformat-get-openapi.md
- name: New Relic Get Components Component  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{component_id}/metrics.{format}
  tags: Components, Component, , Metrics., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentscomponent-idmetricsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentscomponent-idmetricsformat-get-openapi.md
- name: New Relic Get Components Component  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///components/{component_id}/metrics/data.{format}
  tags: Components, Component, , Metrics, Data., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentscomponent-idmetricsdataformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/componentscomponent-idmetricsdataformat-get-openapi.md
- name: New Relic Get Key Transactions. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a paginated \nlist of the key transactions
    associated with your New Relic account.  The time range for summary data is the
    last 10 minutes.\n\nKey transactions can be filtered by their name or list of
    IDs.\n\nSee our documentation for a discussion of \nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///key_transactions.{format}
  tags: Key, Transactions., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/key-transactionsformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/key-transactionsformat-get-openapi.md
- name: New Relic Get Key Transactions  . Format
  x-api-slug: new-relic
  description: "This endpoint returns a single key transaction, identified by ID.
    The time range for summary data is the last 10 minutes.\n\nSee our documentation
    for a discussion of \nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///key_transactions/{id}.{format}
  tags: Key, Transactions, , ., Format
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/key-transactionsidformat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/key-transactionsidformat-get-openapi.md
- name: New Relic Get Labels. Format
  x-api-slug: new-relic
  description: This API endpoint returns a paginated list of the labels available
    for the account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels.{format}
  tags: Labels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/labelsformat-get-openapi.md
- name: New Relic Put Labels. Format
  x-api-slug: new-relic
  description: "This API endpoint will create a new label with the provided category
    and name.\n\nInclude the application and server IDs to which the label should
    be applied in the corresponding arrays.\nYou may omit the \u201Clinks\u201D or
    \u201Cservers\u201D arrays, if not needed.\n\nSee our documentation for a discussion
    on obtaining \napplication \nand \nserver IDs."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels.{format}
  tags: Labels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/labelsformat-put-openapi.md
- name: New Relic Delete Labels Key . Format
  x-api-slug: new-relic
  description: |-
    When applications are provided, this endpoint will remove those applications from the label.

    When no applications are provided, this endpoint will remove the label.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///labels/{key}.{format}
  tags: Labels, Key, ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/labelskeyformat-delete-openapi.md
- name: New Relic Get Mobile Applications. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a list of the Mobile Applications associated with your New Relic account.

    MobileApplications can be filtered by their name, or by the application IDs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///mobile_applications.{format}
  tags: Mobile, Applications., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/mobile-applicationsformat-get-openapi.md
- name: New Relic Get Mobile Applications  . Format
  x-api-slug: new-relic
  description: This API endpoint returns a single Mobile Application, identified by
    ID. The time range for summary data is the last 30 minutes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///mobile_applications/{id}.{format}
  tags: Mobile, Applications, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/mobile-applicationsidformat-get-openapi.md
- name: New Relic Get Mobile Applications Mobile Application  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///mobile_applications/{mobile_application_id}/metrics.{format}
  tags: Mobile, Applications, Mobile, Application, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/mobile-applicationsmobile-application-idmetricsformat-get-openapi.md
- name: New Relic Get Mobile Applications Mobile Application  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///mobile_applications/{mobile_application_id}/metrics/data.{format}
  tags: Mobile, Applications, Mobile, Application, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/mobile-applicationsmobile-application-idmetricsdataformat-get-openapi.md
- name: New Relic Get Notification Channels. Format
  x-api-slug: new-relic
  description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
    API endpoint returns a paginated \nlist of the notification channels associated
    with your New Relic account.\n\nNotification channels can be filtered by their
    type or a list of IDs."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///notification_channels.{format}
  tags: Notification, Channels., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/notification-channelsformat-get-openapi.md
- name: New Relic Get Notification Channels  . Format
  x-api-slug: new-relic
  description: "WARNING: This is legacy alerting.  This endpoint will be deprecated.\n\nThis
    API endpoint returns a single notification channel, identified by ID.\u201D"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///notification_channels/{id}.{format}
  tags: Notification, Channels, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/notification-channelsidformat-get-openapi.md
- name: New Relic Get Plugins. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of the Plugins associated with your
    New Relic account.\n\nPlugins can be filtered by their guid or the list of plugin
    IDs.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///plugins.{format}
  tags: Plugins., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/pluginsformat-get-openapi.md
- name: New Relic Get Plugins  . Format
  x-api-slug: new-relic
  description: This API endpoint returns a single plugin, identified by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///plugins/{id}.{format}
  tags: Plugins, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/pluginsidformat-get-openapi.md
- name: New Relic Get Servers. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a paginated
    list of the Servers associated with your New Relic account. The time range for summary data is the last 10 minutes.

    Servers can be filtered by their name, hostname, or the list of server IDs.

    See our documentation for a discussion and examples of
    using filters
    and summary data output.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers.{format}
  tags: Servers., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversformat-get-openapi.md
- name: New Relic Get Servers  . Format
  x-api-slug: new-relic
  description: "This API endpoint returns a single Server, identified by ID. The time
    range for summary data is the last 10 minutes.\u201D\n\nSee our documentation
    for a discussion on\nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversidformat-get-openapi.md
- name: New Relic Put Servers  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint allows you to rename your server.

    The input is expected to be in JSON or XML format in the body parameter of the PUT request. The exact
    schema is defined below. Any extra parameters passed in the body will be ignored.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversidformat-put-openapi.md
- name: New Relic Delete Servers  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint deletes a server and all of its reported data.

    WARNING: Only servers that have stopped reporting can be deleted. This is an irreversible process which
    will delete all reported data for this server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversidformat-delete-openapi.md
- name: New Relic Get Servers Server  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{server_id}/metrics.{format}
  tags: Servers, Server, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversserver-idmetricsformat-get-openapi.md
- name: New Relic Get Servers Server  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{server_id}/metrics/data.{format}
  tags: Servers, Server, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/serversserver-idmetricsdataformat-get-openapi.md
- name: New Relic Get Usages Product . Format
  x-api-slug: new-relic
  description: |-
    Show a list of usage for a product in a given time frame.

    NOTE: Currently you must request 1 month of data, or less, to retrieve daily usage. Requests for greater than 1 month will currently return only monthly usage.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///usages/{product}.{format}
  tags: Usages, Product, ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/usagesproductformat-get-openapi.md
- name: New Relic Get Users. Format
  x-api-slug: new-relic
  description: |-
    Show a paginated list of all users.

    Uers can be filtered by their ids or email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users.{format}
  tags: Users., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/usersformat-get-openapi.md
- name: New Relic Get Users  . Format
  x-api-slug: new-relic
  description: This API endpoint returns a single user, identified by ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users/{id}.{format}
  tags: Users, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/usersidformat-get-openapi.md
- name: New Relic Add Users  Reset Password. Format
  x-api-slug: new-relic
  description: This API endpoints reset the user password, identified by ID
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///users/{id}/reset_password.{format}
  tags: Users, , Reset, Password., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/usersidreset-passwordformat-post-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: "New Relic\u2019s digital intelligence platform lets developers, ops,
    and tech teams measure and monitor the performance of their applications and infrastructure."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: New Relic
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/new-relic/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---