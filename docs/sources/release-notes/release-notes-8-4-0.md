+++
title = "Release notes for Grafana 8.4.0"
hide_menu = true
+++

<!-- Auto generated by update changelog github action -->

# Release notes for Grafana 8.4.0

### Features and enhancements

- **API:** Extract OpenAPI specification from source code using go-swagger. [#40528](https://github.com/grafana/grafana/pull/40528), [@papagian](https://github.com/papagian)
- **AccessControl:** Disable user remove and user update roles when they do not have the permissions. [#43429](https://github.com/grafana/grafana/pull/43429), [@Jguer](https://github.com/Jguer)
- **AccessControl:** Provisioning for teams. [#43767](https://github.com/grafana/grafana/pull/43767), [@gamab](https://github.com/gamab)
- **API:** Add usage stats preview endpoint. [#43899](https://github.com/grafana/grafana/pull/43899), [@Jguer](https://github.com/Jguer)
- **Alerting:** Move slow queries in the scheduler to another goroutine. [#44423](https://github.com/grafana/grafana/pull/44423), [@grobinson-grafana](https://github.com/grobinson-grafana)
- **Alerting:** Use time.Ticker instead of alerting.Ticker in ngalert. [#44395](https://github.com/grafana/grafana/pull/44395), [@grobinson-grafana](https://github.com/grobinson-grafana)
- **Alerting:** add custom grouping to Alert Panel. [#44559](https://github.com/grafana/grafana/pull/44559), [@gillesdemey](https://github.com/gillesdemey)
- **Analytics:** Add user id tracking to google analytics. [#42763](https://github.com/grafana/grafana/pull/42763), [@autoric](https://github.com/autoric)
- **Angular:** Add AngularJS plugin support deprecation plan to docs site. [#45149](https://github.com/grafana/grafana/pull/45149), [@torkelo](https://github.com/torkelo)
- **Auth:** implement auto_sign_up for auth.jwt. [#43502](https://github.com/grafana/grafana/pull/43502), [@sakjur](https://github.com/sakjur)
- **Azure Monitor Logs:** Order subscriptions in resource picker by name. [#45228](https://github.com/grafana/grafana/pull/45228), [@sunker](https://github.com/sunker)
- **Azure monitor Logs:** Optimize data fetching in resource picker. [#44549](https://github.com/grafana/grafana/pull/44549), [@sunker](https://github.com/sunker)
- **AzureMonitor:** Filter list of resources by resourceType. [#43522](https://github.com/grafana/grafana/pull/43522), [@andresmgot](https://github.com/andresmgot)
- **BarChart:** color by field, x time field, bar radius, label skipping. [#43257](https://github.com/grafana/grafana/pull/43257), [@leeoniya](https://github.com/leeoniya)
- **Chore:** Implement OpenTelemetry in Grafana. [#42674](https://github.com/grafana/grafana/pull/42674), [@idafurjes](https://github.com/idafurjes)
- **Cloud Monitoring:** Adds metric type to Metric drop down options. [#43268](https://github.com/grafana/grafana/pull/43268), [@tw1nk](https://github.com/tw1nk)
- **CloudWatch:** Add Data Lifecycle Manager metrics and dimension. [#43310](https://github.com/grafana/grafana/pull/43310), [@ilyastoli](https://github.com/ilyastoli)
- **CloudWatch:** Add Missing Elasticache Host-level metrics. [#43455](https://github.com/grafana/grafana/pull/43455), [@dhendo](https://github.com/dhendo)
- **CloudWatch:** Add all ElastiCache Redis Metrics. [#43336](https://github.com/grafana/grafana/pull/43336), [@siavashs](https://github.com/siavashs)
- **CloudWatch:** Add new AWS/ES metrics. [#43034](https://github.com/grafana/grafana/pull/43034), [@sunker](https://github.com/sunker)
- **Cloudwatch:** Add syntax highlighting and autocomplete for "Metric Search". [#43985](https://github.com/grafana/grafana/pull/43985), [@sarahzinger](https://github.com/sarahzinger)
- **Explore:** Support custom display label for exemplar links for Prometheus datasource. [#42732](https://github.com/grafana/grafana/pull/42732), [@JokerQueue](https://github.com/JokerQueue)
- **Hotkeys:** Make time range absolute/permanent. [#43802](https://github.com/grafana/grafana/pull/43802), [@davkal](https://github.com/davkal)
- **Playlists:** Enable sharing direct links to playlists. [#44161](https://github.com/grafana/grafana/pull/44161), [@ashharrison90](https://github.com/ashharrison90)
- **SQLStore:** Prevent concurrent migrations. [#44101](https://github.com/grafana/grafana/pull/44101), [@papagian](https://github.com/papagian)
- **SSE:** Add Mode to drop NaN/Inf/Null in Reduction operations. [#43583](https://github.com/grafana/grafana/pull/43583), [@kylebrandt](https://github.com/kylebrandt)
- **Setting:** Support configuring feature toggles with bools instead of just passing an array. [#43326](https://github.com/grafana/grafana/pull/43326), [@bergquist](https://github.com/bergquist)
- **TimeSeries:** Add support for negative Y and constant transform. [#44774](https://github.com/grafana/grafana/pull/44774), [@dprokop](https://github.com/dprokop)
- **Transformations:** Add 'JSON' field type to ConvertFieldTypeTransformer. [#42624](https://github.com/grafana/grafana/pull/42624), [@sd2k](https://github.com/sd2k)

### Bug fixes

- **Auth:** Guarantee consistency of signed SigV4 headers. [#45054](https://github.com/grafana/grafana/pull/45054), [@wbrowne](https://github.com/wbrowne)
- **CloudWatch:** Fix MetricName resetting on Namespace change. [#44165](https://github.com/grafana/grafana/pull/44165), [@yaelleC](https://github.com/yaelleC)
- **Cloudwatch :** Fixed resetting metric name when changing namespace in Metric Query. [#44612](https://github.com/grafana/grafana/pull/44612), [@yaelleC](https://github.com/yaelleC)
- **Explore:** Avoid locking timepicker when range is inverted. [#44790](https://github.com/grafana/grafana/pull/44790), [@Elfo404](https://github.com/Elfo404)
- **Instrumentation:** Fix HTTP request instrumentation of authentication failures. [#44234](https://github.com/grafana/grafana/pull/44234), [@marefr](https://github.com/marefr)
- **LibraryPanels:** Prevent long descriptions and names from obscuring the delete button. [#45190](https://github.com/grafana/grafana/pull/45190), [@zuchka](https://github.com/zuchka)
- **OAuth:** Fix parsing of ID token if header contains non-string value. [#44159](https://github.com/grafana/grafana/pull/44159), [@marefr](https://github.com/marefr)
- **Panel Edit:** Visualization search now works correctly with special characters. [#45137](https://github.com/grafana/grafana/pull/45137), [@ashharrison90](https://github.com/ashharrison90)
- **Provisioning:** Fix duplicate validation when multiple organizations have been configured. [#44151](https://github.com/grafana/grafana/pull/44151), [@marefr](https://github.com/marefr)
- **QueryField:** Fix issue with undo history when suggestion is inserted (#28656). [#39114](https://github.com/grafana/grafana/pull/39114), [@glintik](https://github.com/glintik)
- **TablePanel:** Do not prefix columns with frame name if multiple frames and override active. [#45174](https://github.com/grafana/grafana/pull/45174), [@mdvictor](https://github.com/mdvictor)

### Deprecations

AngularJS plugin support is now in a deprecated state, meaning it will be removed in a future release. Currently, that is planned for version 10 (in 2023). The documentation site has an [article](https://grafana.com/docs/grafana/next/developers/angular_deprecation/) with more details on why, when, and how. Issue [#45149](https://github.com/grafana/grafana/issues/45149)