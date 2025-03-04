## 1.77.3 (August 16, 2022)

ENHANCEMENTS:

* resource `tencentcloud_tem_gateway` output `vip` and `clb_id`

DEPRECATED:

* resource `tencentcloud_clb_target_group` deprecated `target_group_instances`

## 1.77.2 (August 15, 2022)

FEATURES:

* new resource `tencentcloud_cdn_domain_verifier`

ENHANCEMENTS:

* resource `tencentcloud_tem_workload` discard `reserved` config change
* resource `tencentcloud_tem_log_config` and `tencentcloud_tem_scale_rule` add param `workload_id`
* resource `tencentcloud_instances_set` add hint for not support change `instance_count`

## 1.77.1 (August 12, 2022)

ENHANCEMENTS:

* resource `tencentcloud_tem_workload` support update
* resource `tencentcloud_security_group_rule` support policy index

## 1.77.0 (August 11, 2022)

FEATURES:

* new resource `tencentcloud_tem_environment`
* new resource `tencentcloud_tem_application`
* new resource `tencentcloud_tem_workload`
* new resource `tencentcloud_tem_app_config`
* new resource `ttencentcloud_tem_log_config`
* new resource `tencentcloud_tem_scale_rule`
* new resource `tencentcloud_tem_gateway`

ENHANCEMENTS:

* resource `tencentcloud_cdn_domain` support `tls_versions`
* resource `tencentcloud_cbs_storage` skip prepaid upgrade testcase
* resource `tencentcloud_cos_bucket` make policy header to schema set
* resource `tencentcloud_cos_bucket_policy` fix testcase
* resource `tencentcloud_kubernetes_cluster` add node ready checking
* resource `tencentcloud_kubernetes_cluster_endpoint` add node ready checking
* resource `tencentcloud_kubernetes_node_pool` support multi_zone_subnet_policy modify
* resource `tencentcloud_postgresql_instance` increase waiting timeout
* resource `tencentcloud_sqlserver_publish_subscribe` optimize testcase sweepe
* service `service_tencentcloud_as` cancel deprecated asg relative api

BUGFIXES:

* resource `tencentcloud_postgresql_instance` fix npe

## 1.76.4 (August 1, 2022)

ENHANCEMENTS:

* datasource `tencentcloud_cfs_file_systems` output support `mount_ip`

BUGFIXES:

* resource`tencentcloud_as_scaling_group` clear as retry capture

## 1.76.3 (July 25, 2022)

ENHANCEMENTS:

* resource `tencentcloud_clb_listener` support `target_type`
* datasource `tencentcloud_images ` support `instance_type`

DEPRECATED:

* resource `tencentcloud_kubernetes_cluster` deprecated `as_enabled`

BUGFIXES:

* resource `tencentcloud_kubernetes_cluster` fix `cluster_level` desc

## 1.76.2 (July 22, 2022)

FEATURES:

* New resource `tencentcloud_monitor_tmp_scrape_job`
* New resource `tencentcloud_monitor_tmp_tke_alert_policy`
* New resource `tencentcloud_monitor_tmp_exporter_integration`

DEPRECATED:

* resource `tencentcloud_kubernetes_cluster_endpoint`, `tencentcloud_kubernetes_cluster` the
  argument `managed_cluster_internet_security_policies` was deprecated

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_cluster` and data source `tencentcloud_kubernetes_clusters` support output private
  kube config

BUGFIXES:

* resource `tencentcloud_kubernetes_cluster` fix cluster intranet subnet modification limit
* resource `tencentcloud_security_group_lite_rule`, `tencentcloud_monitor_tmp_cvm_agent`
  , `tencentcloud_monitor_tmp_instance` fix example codes.

COMMON:

* resource `tencentcloud_postgresql_instance` fix testcases.

## 1.76.1 (July 21, 2022)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_cluster`, `tencentcloud_kubernetes_cluster_endpoint`
  support `cluster_internet_security_group`
* resource `tencentcloud_cdn_domain` extend multiple unsupport params.

## 1.76.0 (July 13, 2022)

ENHANCEMENTS:

* resource `tencentcloud_clb_attachment` support `eni_ip` for `target`

BUGFIXES:

* resource `tencentcloud_gaap_realserver` fix tag for loop mismatch

COMMON:

* document - add data type for every argument description
* fix clb, cls, vod, key-pair testcases
* service `service_tencentcloud_cvm` add max thread concurrent num

## 1.75.7 (July 08, 2022)

ENHANCEMENTS:

* resource `tencentcloud_monitor_tmp_alert_rule` update docs

## 1.75.6 (July 08, 2022)

FEATURES:

* new resource `tencentcloud_monitor_tmp_instance`
* new resource `tencentcloud_monitor_tmp_cvm_agent`
* new resource `tencentcloud_monitor_tmp_alert_rule`
* new resource `tencentcloud_monitor_tmp_recording_rule`
* new resource `tencentcloud_monitor_tmp_tke_template`
* new resource `tencentcloud_kubernetes_cluster_endpoint`

ENHANCEMENTS:

* resource `tencentcloud_ssl_certificate` support tags

## 1.75.5 (July 01, 2022)

ENHANCEMENTS:

* datasource `tencentcloud_instances_set`  hard check `instance_count` either equal
* datasource `tencentcloud_cbs_storages_set` hard check `disk_count` either equal

## 1.75.4 (July 01, 2022)

FEATURES:

* new datasource `tencentcloud_instances_set`
* new datasource `tencentcloud_cbs_storages_set`

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_cluster` support encrypt disk

## 1.75.3 (June 30, 2022)

FEATURES:

* new datasource `tencentcloud_ckafka_instances`

ENHANCEMENTS:

* resource `tencentcloud_instance_set` add timeout
* datasource `tencentcloud_instance` add field `instances_ids`
* resource `tencentcloud_ckafka_instance` support vips

## 1.75.2 (June 29, 2022)

FEATURES:

* new resource `tencentcloud_cbs_storage_set`

## 1.75.1 (June 28, 2022)

ENHANCEMENTS:

* resource `tencentcloud_instance_set` update docs

## 1.75.0 (June 28, 2022)

FEATURES:

* new resource `tencentcloud_instance_set`

ENHANCEMENTS:

* resource `tencentcloud_monitor_alarm_policy` optimize errors

## 1.74.3 (June 24, 2022)

ENHANCEMENTS:

* resource `tencentcloud_cls_machine_group` update tags
* resource `tencentcloud_kubernetes_node_pool` fix node count

## 1.74.2 (June 23, 2022)

FEATURES:

* new resource `tencentcloud_ssl_free_certificate`
* new resource `tencentcloud_clb_snat_ip`

ENHANCEMENTS:

* resource `tencentcloud_vpn_connection` support healthcheck
* resource `tencentcloud_postgresql_instance` add plan modify retry
* resource `tencentcloud_cdn_domain` support follow redirect and authentication
* resource `tencentcloud_redis_instance` update redis_shard_num
* resource `tencentcloud_clb_instance` support snat pro and snat ips
* resource `tencentcloud_cls_topic` update storage_type, auto_split, partition_count
* resource `tencentcloud_cls_logset` update tags

## 1.74.1 (June 20, 2022)

ENHANCEMENTS:

* resource `tencentcloud_kms_key` optimize kms key disable logic

## 1.74.0 (June 20, 2022)

FEATURES:

* New resource `tencentcloud_cdn_url_purge`
* New resource `tencentcloud_cdn_url_push`

ENHANCEMENTS:

* resource `tencentcloud_cam_role` support tags
* resource `tencentcloud_cam_user` support tags
* resource `tencentcloud_kms_key` optimize delete logic
* resource `tencentcloud_kubernetes_cluster` optimize cluster_level logic

COMMON:

* fix vod testcases

## 1.73.3 (June 16, 2022)

FEATURES:

* datasourcce `tencentcloud_user_info` support get userinfo

BUGFIXES:

* resource `resource_tc_cls_index` fix crash error
* resource `resource_tc_clb_instance` fix tag error
* resource `resource_tc_kubernetes_cluster` fix cluster_level error

COMMON:

* fix cls, cfs testcases

## 1.73.2 (June 13, 2022)

BUGFIXES:

* resource `tencentcloud_clb_attachment` disable target diff if using TCP-SSL listener
* resource `tencentcloud_instance` support prepaid/postpaid charge type dual modify

COMMON:

* fix gaap, cvm datasource testcases

## 1.73.1 (June 09, 2022)

ENHANCEMENTS:

* resource `tencentcloud_instance` remove unnecessary retries and optimize state management on launch failed cvm

## 1.73.0 (June 08, 2022)

FEATURES:

* new resource `tencentcloud_cls_index`
* new resource `tencentcloud_lighthouse_instance`

ENHANCEMENTS:

* resource `tencentcloud_dc_gateway` add protect sleep
* resource `tencentcloud_kubernetes_cluster` fix docs

COMMON:

* fix testcases

## 1.72.8 (June 02, 2022)

ENHANCEMENTS:

* resource `tencentcloud_mysql_instance` support device type
* resource `tencentcloud_mysql_readonly_instance` support device type

COMMON:

* resource `tencentcloud_tcaplus_table` add test sweeper
* chore: add changelog draft script

## 1.72.7 (May 31, 2022)

BUGFIXES:

* resource `tencentcloud_mysql_readonly_instance` make zone arguments optional.

## 1.72.6 (May 31, 2022)

FEATURES:

* new resource `tencentcloud_cam_role_sso`

ENHANCEMENTS:

* resource `tencentcloud_mysql_instance`  support fast upgrade and param template id

BUGFIXES:

* resource `tencentcloud_sqlserver_instance` disable recycle
* resource `tencentcloud_mysql_instance` / `tencentcloud_mongodb_instance` cancel validate required db pwd.

COMMON:

* testcases fix: dnspod, cvm, kafka, as, tcr, sqlserver, cbs, cos, cfs, mongo, tke

## 1.72.5 (May 20, 2022)

ENHANCEMENTS:

* resource `tencentcloud_ckafka_instance` support upgrade config
* resource `tencentcloud_kubernetes_cluster` support log agent/audit/event persistence

## 1.72.4 (May 18, 2022)

ENHANCEMENTS:

* resource `tencentcloud_vpn_gateway` add `cdc_id` and `max_connection`
* resource `tencentcloud_private_dns_zone` support tag change
* resource `tencentcloud_route_table_entry` add disabled argument
* datasource `tencentcloud_cbs_storages` support more query filters

BUGFIXES:

* resource `tencentcloud_private_dns_record` fix delete error

COMMON:

* fix testcases

## 1.72.3 (May 13, 2022)

ENHANCEMENTS:

* resource `tencentcloud_gaap_http_rule` add `sni` and `sni_switch`
* resource `tencentcloud_scf_function` remove memSize validate

## 1.72.2 (May 11, 2022)

BUGFIXES:

* resource `tencentcloud_mysql_readonly_instance` skip monitor check.
* resource `tencentcloud_clb_listener_rule` fix domain and port update.
* resource `tencentcloud_kubernetes_cluster` add cluster level modify retry.

COMMON:

* fix testcases

## 1.72.1 (May 6, 2022)

ENHANCEMENTS:

* resource `tencentcloud_scf_function` support java handler
* resource `tencentcloud_mongodb_instance` fix engine version doc

## 1.72.0 (May 5, 2022)

FEATURES:

* New datasource `tencentcloud_kubernetes_cluster_common_names`
* New resource `tencentcloud_cam_oidc_sso`

ENHANCEMENTS:

* resource `tencentcloud_postgresql_instance` support data transparent encryption

BUGFIXES:

* resource `tencentcloud_vpn_ssl_client` fix delete failed
* resource `tencentcloud_vpn_ssl_server` fix create duplicate instance

## 1.71.0 (April 24, 2022)

FEATURES:

* New datasource `tencentcloud_postgresql_xlogs`

ENHANCEMENTS:

* resource `tencentcloud_postgresql_instance` support backup plan
* resource `tencentcloud_redis_instance` support `replica_zone_ids` modify

BUGFIXES:

* resource `tencentcloud_eks_cluster` fix LB modified errors

## 1.70.3 (April 22, 2022)

ENHANCEMENTS:

* resource `tencentcloud_ckafka_instance` remove validate check
* resource `tencentcloud_tcr_vpc_attachment` modify doc

## 1.70.2 (April 21, 2022)

FEATURES:

* New resource `tencentcloud_cls_config_extra`

BUGFIXES:

* resource `tencentcloud_cls_topic` plan change
* resource `tencentcloud_cls_config` create failed when log_type is full regex

## 1.70.1 (April 19, 2022)

BUGFIXES:

* resource `tencentcloud_ckafka_instance` plan change
* resource `tencentcloud_mysql_instance`  ignore lowercase when 8.0

## 1.70.0 (April 19, 2022)

BUGFIXES:

* New resource `tencentcloud_cls_config`
* New resource `tencentcloud_cls_config_attachment`

## 1.69.0 (April 19, 2022)

FEATURES:

* New resource `tencentcloud_cls_config`
* New resource `tencentcloud_cls_config_attachment`

## 1.68.0 (April 12, 2022)

FEATURES:

* New resource `tencentcloud_cls_cos_shipper`
* New resource `tencentcloud_postgresql_readonly_instance`
* New resource `tencentcloud_postgresql_readonly_group`
* New resource `tencentcloud_postgresql_readonly_attachment`

BUGFIXES:

* resource `tencentcloud_elasticsearch_instance` support `web_node_type_info` modify

COMMON

* update es, eks(ci), myqsl, redis, sqlserver sweepers

## 1.67.0 (April 8, 2022)

FEATURES:

* New resource `tencentcloud_cls_logset`
* New resource `tencentcloud_cls_topic`
* New resource `tencentcloud_cls_machine_group`

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_cluster` support cluster level and auto upgrade level settings.
* resource `tencentcloud_emr_cluster` support `extend_fs_field`

BUGFIXES:

* resource `tencentcloud_emr_cluster` clear metadb
* resource `tencentcloud_instance` ignore local disk describe status.

COMMON:

* fix partial testcases gaap, tke, clb, cam, emr, e.g.

## 1.66.3 (March 31, 2022)

BUGFIXES:

* resource `tencentcloud_sqlserver_instance` block name mistake in example block.
* resource `tencentcloud_kubernetes_node_pool`, `tencentcloud_kubernetes_cluster_attachment`
  fix `data_disk.disk_partition` usage description.

ENHANCEMENTS:

* resource `tencentcloud_as_scaling_config` support prepaid and spot charge type.
* resource `tencentcloud_ckafka_config` support multi zones config.

## 1.66.2 (March 31, 2022)

BUGFIXES:

* resource `tencentcloud_instance` optimize charge type modification.
* resource `tencentcloud_postgresql_instance` fix instance upgrade polling error.
* resource `tencentcloud_vpn_ssl_client`
* fix vpc, vpngw, clb and eni testcases.

ENHANCEMENTS:

* resource `tencentcloud_sqlserver_instance`,`tencentcloud_sqlserver_readonly_instance` support prepaid charge type

## 1.66.1 (March 24, 2022)

BUGFIXES:

* resource `tencentcloud_elasticsearch_instance` testcases.

ENHANCEMENTS:

* resource `tencentcloud_mysql_readonly_instance` support cross-zone purchase and query remoteRoZones
* resource `tencentcloud_scf_function` support cfs config and fix testcases
* resource `tencentcloud_eks_cluster` support output kubeconfig
* resource `tencentcloud_emr_cluster` support `root_size` and `sg_id` params.

## 1.66.0 (March 22, 2022)

FEATURES:

* new datasource `tencentcloud_eks_cluster_credential`

ENHANCEMENTS:

* resource `tencentcloud_eks_cluster` support public and internal load balancer config

BUGFIXES:

* resource `tencentcloud_instance` charge type update then polling status mismatch

## 1.65.2 (March 18, 2022)

ENHANCEMENTS:

* resource `tencentcloud_route_entry` extend next type
* resource `tencentcloud_clb_instance` create with tag params
* resource `tencentcloud_emr_cluster` support need_master_wan param
* resource `tencentcloud_cos_bucket` support lifecycle rule id and delete marker
* resource `tencentcloud_mysql_readonly_instance` support zone param

BUGFIXES:

* testcases: cvm, cynosdb, eks, mysql, vpn
* resource `tencentcloud_emr_cluster` destroy
* resource `tencentcloud_mysql_instance` init
* resource `tencentcloud_redis_instance` reset pwd retry and comment

## 1.65.1 (March 14, 2022)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_node_pool` data_disk support `delete_with_instance` option
* resource `tencentcloud_as_scaling_configs` data_disk support `delete_with_instance` option
* datasource `tencentcloud_as_scaling_configs` data_disk add `delete_with_instance` field

BUGFIXES:

* testcases fixes: CVM,SG,MySQL,EKS
* testcases tke use preset tke and tlinux image instead

## 1.65.0 (March 7, 2022)

FEATURES:

* new datasource `tencentcloud_dnspod_record`
* new resource `tencentcloud_vpn_ssl_server`
* new resource `tencentcloud_vpn_ssl_client`

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_node_pool` support `cam_role_name` as parameter

## 1.64.0 (March 7, 2022)

FEATURES:

* new datasource `tencentcloud_mysql_default_params`
* new resource `tencentcloud_dayu_cc_policy_v2`

BUGFIXES:

* resource `tencentcloud_mysql_instance` init database after create
* resource `tencentcloud_emr_cluster` pay_mode can not use 0
* testcases - add vpngw sweeper and fix cvm sweeper

ENHANCEMENTS:

* resource `tencentcloud_cynosdb_cluster` support `param_items` as parameter

## 1.63.0 (March 2, 2022)

FEATURES:

* new resource `tencentcloud_user_info`

BUGFIXES:

* resource `tencentcloud_instance` support data disk `delete_with_instance` on cvm remove
* resource `tencentcloud_redis_instance` support `replicas_read_only

## 1.62.0 (March 1, 2022)

FEATURES:

* new resource `tencentcloud_dayu_ddos_policy_v2`

BUGFIXES:

* datasource `tencentcloud_postgresql_instances` fix query id parameter
* resource `tencentcloud_cynosdb_cluster` make `storage_limit` optional and update description

DEPRECATED:

* datasource `tencentcloud_redis_zone_config`: The argument `mem_sizes` was deprecated, use `shard_memories` instead.

## 1.61.13 (February 24, 2022)

ENHANCEMENTS:

* resource `tencentcloud_redis_instance` support `auto_renew_flag`.

## 1.61.12 (February 23, 2022)

ENHANCEMENTS:

* resource `tencentcloud_instance` fix testcase default image

## 1.61.11 (February 23, 2022)

ENHANCEMENTS:

* resource `tencentcloud_instance` support System Disk size and DiskType modification

## 1.61.10 (February 22, 2022)

ENHANCEMENTS:

* resource `tencentcloud_instance` support Data Disk size modification
* resource generic gaap support client_ip_method

## 1.61.9 (February 21, 2022)

ENHANCEMENTS:

* resource `tencentcloud_cos_bucket` support Multi-AZ bucket import, Non-Current Version Lifecycle and ACL body

## 1.61.8 (February 17, 2022)

ENHANCEMENTS:

* resource `tencentcloud_as_scaling_group` support Service Settings

BUGFIXES:

* resource `tencentcloud_mysql_privilege` update global privileges check
* Fix testcases COS Bucket

## 1.61.7 (February 15, 2022)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_node_pool` support CVM instance charge type

BUGFIXES:

* Fix testcases CamPolicies
* Fix testcases CamRole
* Fix testcases TcaplusDB
* Fix testcases EKSCluster

## 1.61.6 (February 5, 2022)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_node_pool` support set `multi_zone_subnet_policy`

## 1.61.5 (January 29, 2022)

ENHANCEMENTS:

* resource `tencentcloud_redis_instance` remove change redis mem_size limit

## 1.61.4 (January 27, 2022)

ENHANCEMENTS:

* resource `tencentcloud_dayu_eip` support create new ddos eip rules
* resource `tencentcloud_dayu_l4_rule_v2` support create new ddos l4 rules
* resource `tencentcloud_dayu_l7_rule_v2` support create new ddos l7 rules
* data source `tencentcloud_dayu_eip` support query new ddos eip rules
* data source `tencentcloud_dayu_l4_rules_v2` support query new ddos l4 rules
* data source `tencentcloud_dayu_l7_rules_v2` support query new ddos l7 rules

## 1.61.3 (January 25, 2022)

ENHANCEMENTS:

* resource `tencentcloud_as_scaling_config` support `instance_name_settings` and `cam_role_name`.

## 1.61.2 (January 21, 2022)

COMMON:

* testcase fix `defaultGaapProxyId`

ENHANCEMENTS:

* resource `tencentcloud_postgresql_instance` support `db_node_set` for multiple available zone.

## 1.61.1 (January 14, 2022)

ENHANCEMENTS:

* resource `tencentcloud_monitor_alarm_policy` support policy tag

## 1.61.0 (January 11, 2022)

COMMON:

* add env variable `TENCENTCLOUD_READ_RETRY_TIMEOUT`  and `TENCENTCLOUD_WRITE_RETRY_TIMEOUT`

BUGFIXES:

* resource `tencentcloud_gaap_proxy` fix destroy error

## 1.60.27 (January 11, 2022)

COMMON:

* add `terraform {}` block to provider doc example
* add `pre-commit` status check

BUGFIXES:

* resource `tencentcloud_scf_function` add COS trigger `bucketUrl` field
* resource `tencentcloud_eip` fix NAT gateway detach error
* service `tencentcloud_gaap` destroy error

ENHANCEMENTS:

* resource `tencentcloud_vpc` add assistant CIDR
* resource `tencentcloud_cos_bucket` support bucket replication

## 1.60.26 (January 6, 2022)

COMMON:

* fix testcases

ENHANCEMENTS:

* resource `tencentcloud_vpc` support vpc assistant CIDR
* resource `tencentcloud_eip` support create HighQualityEIP
* resource `tencentcloud_instance` support charge type update

## 1.60.25 (December 27, 2021)

BUGFIXES:

* Resource `tencentcloud_instance` rollback instance_charge_type_prepaid_period

## 1.60.24 (December 27, 2021)

COMMON:

* add testcases basic required resource

BUGFIXES:

* fix service mongodb status query

## 1.60.23 (December 24, 2021)

ENHANCEMENTS:

* resource `tencentcloud_vpn_gateway` improve timeout min

BUGFIXES:

* Resource `tencentcloud_postgresql_instance` fix computed attribute uid get 0
* Resource `tencentcloud_monitor_alarm_policy` fix filter when has event condition

## 1.60.22 (December 21, 2021)

ENHANCEMENTS:

* resource `tencentcloud_mysql_readonly_instance` fix create prepaid instance

## 1.60.21 (December 20, 2021)

FEATURES:

* **New Resource**: `tencentcloud_private_dns_record`

ENHANCEMENTS:

* resource `tencentcloud_postgresql_instance` add computed attribute uid

## 1.60.20 (December 16, 2021)

ENHANCEMENTS:

* resource `tencentcloud_monitor_alarm_policy` fix filter bug
* resource `tencentcloud_clb_customized_config` remove content length validate
* resource `tencentcloud_ckafka_instance` modify docs

## 1.60.19 (December 16, 2021)

FEATURES:

* **New Resource**: `tencentcloud_ckafka_instance`

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_addon_attachment` add tcr example values
* resource  `tencentcloud_instance` support cvm import params
* datasource `tencentcloud_kubernetes_charts`fix domain 404

## 1.60.18 (December 10, 2021)

ENHANCEMENTS:

* resource `tencentcloud_redis_instance` support no-auth access

## 1.60.17 (December 9, 2021)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_cluster` modify docs.
* resource `tencentcloud_kubernetes_cluster` ignore `ImageId` JSON if user make it empty.
* resource `tencentcloud_cbs_storage` remove `CLOUD_BASIC` type
* resource `tencentcloud_postgresql_instance` change available versions
* resource `tencentcloud_postgresql_instance` support `max_standby_*` params

## 1.60.16 (December 3, 2021)

ENHANCEMENTS:

* resource `tencentcloud_kubernetes_addon_attachment` fix tke_addon - npe error

## 1.60.15 (December 3, 2021)

FEATURES:

* **New Datasource** `tencentcloud_kubernetes_charts`
* **New Resource** `tencentcloud_kubernetes_addon_attachment`

## 1.60.14 (December 2, 2021)

ENHANCEMENTS:

* resource `resource_tc_monitor_alarm_policy` support change name and remark

## 1.60.13 (December 1, 2021)

ENHANCEMENTS:

* resource `resource_tc_security_group_rule`  remove cidr validate
* resource `resource_tc_monitor_alarm_policy` support manage tke rules
* datasource `tencentcloud_instance_types ` support filter by charge type

## 1.60.12 (November 30, 2021)

FEATURES:

* **New Resource**: `tencentcloud_private_dns_zone`

ENHANCEMENTS:

* resource `tencentcloud_monitor_policy_binding_object`  support import
* resource `tencentcloud_kubernetes_cluster` support modify enableClusterDeletionProtection

## 1.60.11 (November 25, 2021)

FEATURES:

* **New Resource**: `tencentcloud_emr_cluster`
* **New Resource**: `tencentcloud_clb_customized_config`

BUGFIXES:

* Resource `tencentcloud_kubernetes_node_pool` support launch config attributes modify

## 1.60.10 (November 22, 2021)

FEATURES:

* **New Resource**: `tencentcloud_eks_container_instance`
* **New Resource**: `tencentcloud_dnspod_domain_instance`

BUGFIXES:

* Resource `tencentcloud_monitor_alarm_policy` remove alarm policy binding check

DEPRECATED:

* Disk type `CLOUD_BASIC` which referenced by CVM/TKE/CBS was no longer available

## 1.60.9 (November 16, 2021)

BUGFIXES:

* Resource `tencentcloud_instance` omit `InstanceMarketOptions` field if spot arguments empty

## 1.60.8 (November 16, 2021)

BUGFIXES:

* Resource `tencentcloud_clb_log_set` remove doc

## 1.60.7 (November 16, 2021)

FEATURES:

* **New Resource**: `tencentcloud_clb_log_set`
* **New Resource**: `tencentcloud_clb_log_topic`

ENHANCEMENTS:

* resource `tencentcloud_clb_instance`  support set log
* resource `tencentcloud_instance` unlimited spot charge argument

## 1.60.6 (November 12, 2021)

FEATURES:

* **New Resource**: `tencentcloud_monitor_policy_binding_object`

ENHANCEMENTS:

* fix resource `tencentcloud_kubernetes_node_pool` plan change
* fix resource `tencentcloud_monitor_alarm_policy` import lacking eventditions

DEPRECATED:

* Resource: `tencentcloud_monitor_binding_object` replaced by tencentcloud_monitor_policy_binding_object

## 1.60.5 (November 8, 2021)

BUGFIXES:

*Resource `tencentcloud_availability_zones_by_product` add dependency

## 1.60.4 (November 8, 2021)

FEATURES:

* **New Resource**: `tencentcloud_vod_sub_application`
* **New Resource**: `tencentcloud_availability_zones_by_product`

ENHANCEMENTS:

* resource `tencentcloud_clb_instance` support set load_balancer_pass_to_target

DEPRECATED:

* Resource: `tencentcloud_availability_zones` replaced by `tencentcloud_availability_zones_by_product`

## 1.60.3 (November 3, 2021)

BUGFIXES:

* Resource `tencentcloud_tcr_repository` fix inaccurate document and example usage

ENHANCEMENTS:

* Resource `tencentcloud_postgresql_instance` support modifying `security_groups`

## 1.60.2 (November 1, 2021)

BUGFIXES:

* resource `tencentcloud_tcr_instance` fix document format error

## 1.60.1 (October 29, 2021)

ENHANCEMENTS:

* resource `tencentcloud_tcr_instance` support security policies

## 1.60.0 (October 28, 2021)

FEATURES:

* **New Resource**: `tencentcloud_scf_layer`

ENHANCEMENTS:

* resource/tencentcloud_scf_function: Add `layers` argument

## 1.59.20 (October 27, 2021)

ENHANCEMENTS:

* resource `tencentcloud_redis_instance` support multi replica zone ids

## 1.59.19 (October 27, 2021)

FEATURES:

* **New Resource**: `tencentcloud_monitor_alarm_policy`

DEPRECATED:

* Resource: `tencentcloud_monitor_policy_group` replaced by `tencentcloud_monitor_alarm_policy`

## 1.59.18 (October 25, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_instance` support instance reset and pay as you go
* Resource `tencentcloud_vpc` support `default_route_table_id`
* DataSource `tencentcloud_vpc_route_tables` add example usage for fetching default route table

DEPRECATED:

* Resource `tencentcloud_instance` argument `instance_count` was deprecated, replace by built-in `count`

## 1.59.17 (October 20, 2021)

BUGFIXES:

* Resource `tencentcloud_vod_xxx` fix resource related to vod, while user create vod resource use sub app id.

## 1.59.16 (October 19, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_clb_instance` support `bandwidth_package_id`

COMMON:

* Resource `tencentcloud_eks_cluster` make essential argument required

## 1.59.15 (October 19, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_scf_function` support scf create by image
* Resource `tencentcloud_security_group_lite_rule` ingress/egress policy support security group ID, address template as
  source

BUGFIXES:

* Resource `tencentcloud_clb_listener` skip empty import set
* Resource `tencentcloud_address_template_group` fix incorrect field `addresses` to `template_ids` in example usage.

## 1.59.14 (October 19, 2021)

BUGFIXES:

* Resource `tencentcloud_kubernetes_auth_attachment` fix official document synchronous error.
* Resource `tencentcloud_elasticsearch_instance` make zone and subnet optional for multi az case.

COMMON:

* Remove outdated go.sum

## 1.59.13 (October 18, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster` support argument `extension_addon`

## 1.59.12 (October 15, 2021)

FEATURES:

* **New Resource**: `tencentcloud_kubernetes_auth_attachment`
* **New Resource**: `tencentcloud_tdmq_instance`
* **New Resource**: `tencentcloud_tdmq_namespace`
* **New Resource**: `tencentcloud_tdmq_topic`
* **New Resource**: `tencentcloud_tdmq_role`
* **New Resource**: `tencentcloud_tdmq_namespace_role_attachment`

## 1.59.11 (October 12, 2021)

FEATURES:

* **New Resource**: `tencentcloud_eks_cluster`
* **New Data Source**: `tencentcloud_eks_clusters`

ENHANCEMENTS:

* Resource `tencentcloud_tcr_vpc_attachment` support argument `region_name`

## 1.59.10 (October, 9, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_cos_bucket_object` support cos object tags.

BUGFIXES:

* Resource `tencentcloud_kubernetes_cluster` update authentication options immediately after create

## 1.59.9 (October, 9, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster` cluster support authentication options.

## 1.59.8 (October, 6, 2021)

BUGFIXES:

* Resource `tencentcloud_tcr_vpc_attachment` pass region_id for delete if provided.

## 1.59.7 (October, 5, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_tcr_vpc_attachment` tcr vpc attachment support region.

## 1.59.6 (September 28, 2021)

BUGFIXES:

* Resource `tencentcloud_kubernetes_node_pool` fix termination_policies argument mistake

DEPRECATED:

* DataSource `data_source_tc_cam_user_policy_attachments` deprecate `user_id` and replaced by `user_name`

## 1.59.5 (September 28, 2021)

ENHANCEMENTS:

* TestCase `TestAccTencentCloudTkeNodePoolResource` extend relative auto-scaling group arguments in node pool resource

DEPRECATED:

* Resource `tencentcloud_cam_group_membership` argument `user_ids` was deprecated, replace by `user_names`
* Resource `tencentcloud_cam_user_policy_attachment` argument `user_id` was deprecated, replace by `user_name`

## 1.59.4 (September 24, 2021)

BUGFIXES:

* Resource `tencentcloud_tcr_instance` support modify tags
* Resource `service_tencentcloud_postgresql` support security group
* Resource `service_tencentcloud_monitor` fix binding policy query limit
* Resource `tencentcloud_api_gateway_api` fix destroy limitNumber

## 1.59.2 (September 18, 2021)

BUGFIXES:

* Add missing AuthorizationTransport.Token field

ENHANCEMENTS:

* Resource `tencentcloud_cdn_domain` support `ipv6_access_switch` config

## 1.59.1 (September 15, 2021)

BUGFIXES:

* Resource `tencentcloud_instance` remove last_update_status judge
* Resource `tencentcloud_instance` fix DescribeInstanceById return LatestOperationState
* Resource `tencentcloud_clb_attachment` clb_attachment check instances before unbind target groups

CHORE:

* Define `TENCENTCLOUD_APPID` Environment variable for testing appid.
* Format code style

## 1.58.5 (September 7, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_redis_backup_config ` change backup_period to optional
* Resource `tencentcloud_scf_function` enable public net config and eip config
* Resource `tencentcloud_cos_bucket` support MAZ, ACL XML body, Origin-Pull rules and origin domain rules

## 1.58.4 (Aug 24, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_node_pool` support `backup_instance_type` for `auto_scaling_config`

## 1.58.3 (Aug 18, 2021)

ENHANCEMENTS:

* Extend kubernetes node instance disk allow types
* Resource `tencentcloud_kubernetes_cluster_attachment` add `disk_partition` field

BUGFIXES:

* Resource `tencentcloud_kubernetes_cluster` fix `auto_format_and_mount` default value to `false`

## 1.58.2 (Aug 18, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster` tke instance creation - add RuntimeVersion param
* Resource `tencentcloud_kubernetes_cluster` extend worker instance data disk mount settings

## 1.58.1 (Aug 17, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_mysql_instance` add cpu params for mysql

BUG FIXES:

* Resource `tencentcloud_instance` fix read cvm data_disks bug

## 1.58.0 (Aug 11, 2021)

FEATURES:

* **New Resource**: `tencentcloud_nat_gateway_snat`
* **New Data Source**: `tencentcloud_nat_gateway_snat`

## 1.57.3 (Aug 10, 2021)

BUG FIXES:

* DataSource `data_source_tc_elasticsearch_instances` skip kibana node info record after elastic search instance create
* Resource `tencentcloud_postgresql_instance` skip kibana node info record after elastic search instance create

## 1.57.2 (Aug 7, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_postgresql_instance` root_user setting support

## 1.57.1 (Aug 5, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_vpn_gateway_route` add example docs

## 1.57.0 (July 28, 2021)

FEATURES:

* **New Resource**: `tencentcloud_vpn_gateway_route`
* **New Data Source**: `tencentcloud_vpn_gateway_route`

## 1.56.15 (July 07, 2021)

BUG FIXES:

* Resource `tencentcloud_tc_kubernetes_cluster` filter the request field of *bandwidth_package_id* when it is null
* Resource `tencentcloud_tc_kubernetes_node_pool` filter the request field of *bandwidth_package_id* when it is null

## 1.56.14 (July 06, 2021)

BUG FIXES:

* Resource `tencentcloud_tc_clb_listener` exec the plan will lead the resource rebuild.

ENHANCEMENTS:

* Resource `tencentcloud_elasticsearch_instance` create **ES** cluster add new parametes of *web_node_type_info*.
* Resource `tencentcloud_tc_instance` add *instance_count* to support create multiple consecutive name of instance
* Resource `tencentcloud_tc_kubernetes_cluster` supports change *internet_max_bandwidth_out*
* Resource `tencentcloud_tc_instance` create cvm instance add *bandwidth_package_id*

## 1.56.13 (July 02, 2021)

BUG FIXES

* Resource `TkeCvmCreateInfo.data_disk.disk_type` support CLOUD_HSSD and CLOUD_TSSD

## 1.56.12 (July 02, 2021)

BUG FIXES

* Resource `TkeCvmCreateInfo.data_disk.disk_type` support CLOUD_HSSD

## 1.56.11

BUG FIXES

* Resource `tencentcloud_kubernetes_cluster` fix create cluster without *desired_pod_num* in tf, then crash
* Resource `tencentcloud_kubernetes_cluster` fix when upgrade terraform-provider-tencentclod from v1.56.1 to newer,
  cluster_os force replacement
* Resource `tencentcloud_kubernetes_cluster` fix when upgrade terraform-provider-tencentclod from v1.56.1 to newer,
  enable_customized_pod_cidr force replace

## 1.56.10

BUG FIXES

* Resource `tencentcloud_tcr_namespace` fix create two namespace and one name is substring of another, then got an error
  about more than 1
* Resource `tencentcloud_tcr_namespace` fix create two repositories and one name is substring of another, then got an
  error about more than 1

## 1.56.9 (Jun 09, 2021)

BUG FIXES:

* Resource `tencentcloud_instance` fix words spell, in tencendcloud/tencentcloud_instance.go L45,
  data.tencentcloud_availability_zones.my_favorate_zones.zones.0.name change to
  data.tencentcloud_availability_zones.my_favorite_zones.zones.0.name".
* Resource `tencentcloud_kubernetes_clusters` fix the description of is_non_static_ip_mode

ENHANCEMENTS:

* Resource `tencentcloud_clb_target_group` add create target group.
* Resource `tencentcloud_clb_instance` add internal CLB supports security group.
* Resource `tencentcloud_clb_instance` add supports open and close CLB security group, default is open.
* Resource `tencentcloud_clb_instance` add external CLB create multi AZ instance.
* Resource `tencentcloud_kubernetes_cluster` add supports params of img_id to assign image.
* Resource `tencentcloud_as_scaling_group` add MultiZoneSubnetPolicy.

## 1.56.8 (May 26, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster_attachment.worker_config` add `desired_pod_num`.
* Resource `tencentcloud_kubernetes_cluster_attachment` add `worker_config_overrides`.
* Resource `tencentcloud_kubernetes_scale_worker` add `desired_pod_num`.
* Resource `tencentcloud_kubernetes_cluster` add `enable_customized_pod_cidr`, `base_pod_num`, `globe_desired_pod_num`,
  and `exist_instance`.
* Resource `tencentcloud_kubernetes_cluster` update available value of `cluster_os`.
* Resource `tencentcloud_as_lifecycle_hook` update `heartbeat_timeout` value ranges.

## 1.56.7 (May 12, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_as_scaling_config` add `disk_type_policy`.
* Data Source `tencentcloud_as_scaling_configs` add `disk_type_policy` as result.

## 1.56.6 (May 7, 2021)

BUG FIXES:

* Resource: `tencentcloud_scf_function` filed `cls_logset_id` and `cls_logset_id` change to Computed.

## 1.56.5 (April 26, 2021)

BUG FIXES:

* Resource: `tencentcloud_kubernetes_cluster` upgrade cluster timeout from 3 to 9 minutes.

## 1.56.4 (April 26, 2021)

BUG FIXES:

* Resource: `tencentcloud_kubernetes_cluster` upgrade instances timeout depend on instance number.

## 1.56.3 (April 25, 2021)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add `upgrade_instances_follow_cluster` for upgrade all instances of
  cluster.

## 1.56.2 (April 19, 2021)

BUG FIXES:

* Remove `ResourceInsufficient` from `retryableErrorCode`.

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` upgrade `cluster_version` will send old `cluster_extra_args` to tke.

## 1.56.1 (April 6，2021)

BUG FIXES:

* Fix release permission denied.

## 1.56.0 (April 2，2021)

FEATURES:

* **New Resource**: `tencentcloud_cdh_instance`
* **New Data Source**: `tencentcloud_cdh_instances`

ENHANCEMENTS:

* Resource: `tencentcloud_instance` add `cdh_instance_type` and `cdh_host_id` to support create instance based on cdh.

## 1.55.2 (March 29, 2021)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add `node_pool_global_config` to support node pool global config setting.

## 1.55.1 (March 26, 2021)

ENHANCEMENTS:

* Resource: `tencentcloud_tcr_vpc_attachment` add more time for retry.

## 1.55.0 (March 26, 2021)

FEATURES:

* **New Resource**: `tencentcloud_ssm_secret`
* **New Resource**: `tencentcloud_ssm_secret_version`
* **New Data Source**: `tencentcloud_ssm_secrets`
* **New Data Source**: `tencentcloud_ssm_secret_versions`

ENHANCEMENTS:

* Resource: `tencentcloud_ssl_certificate` refactor logic with api3.0 .
* Data Source: `tencentcloud_ssl_certificates` refactor logic with api3.0 .
* Resource `tencentcloud_kubernetes_cluster` add `disaster_recover_group_ids` to set disaster recover group ID.
* Resource `tencentcloud_kubernetes_scale_worker` add `disaster_recover_group_ids` to set disaster recover group ID.

## 1.54.1 (March 24, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_tcr_vpc_attachment` add `enable_public_domain_dns`, `enable_vpc_domain_dns` to set whether to
  enable dns.
* Data Source `tencentcloud_tcr_vpc_attachments` add `enable_public_domain_dns`, `enable_vpc_domain_dns`.

## 1.54.0 (March 22, 2021)

FEATURES:

* **New Resource**: `tencentcloud_kms_key`
* **New Resource**: `tencentcloud_kms_external_key`
* **New Data Source**: `tencentcloud_kms_keys`

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster_attachment` add `unschedulable` to set whether the joining node participates
  in the schedule.
* Resource `tencentcloud_kubernetes_cluster` add `unschedulable` to set whether the joining node participates in the
  schedule.
* Resource `tencentcloud_kubernetes_node_pool` add `unschedulable` to set whether the joining node participates in the
  schedule.
* Resource `tencentcloud_kubernetes_scale_worker` add `unschedulable` to set whether the joining node participates in
  the schedule.

## 1.53.9 (March 19, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_tcr_instance` add `open_public_network` to control public network access.
* Resource `tencentcloud_cfs_file_system` add `storage_type` to change file service StorageType.

## 1.53.8 (March 15, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_instance` add `cam_role_name` to support binding role to cvm instance.

BUG FIXES:

* Resource `tencentcloud_instance` fix bug that waiting 5 minutes when cloud disk sold out.
* Resource: `tencentcloud_tcr_instance` fix bug that only one tag is effective when setting multiple tags.

## 1.53.7 (March 10, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_node_pool` add `internet_max_bandwidth_out`, `public_ip_assigned` to support
  internet traffic setting.
* Resource `tencentcloud_instance` remove limit of `data_disk_size`.

## 1.53.6 (March 09, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_eip` support `internet_max_bandwidth_out` modification.
* Resource `tencentcloud_kubernetes_cluster` add `hostname` to support node hostname setting.
* Resource `tencentcloud_kubernetes_scale_worker` add `hostname` to support node hostname setting.

## 1.53.5 (March 01, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_clb_instance` add `internet_charge_type`, `internet_bandwidth_max_out` to support internet
  traffic setting with OPEN CLB instance.
* Resource `tencentcloud_clb_rule` add `http2_switch` to support HTTP2 protocol setting.
* Resource `tencentcloud_kubernetes_cluster` add `lan_ip` to show node LAN IP.
* Resource `tencentcloud_kubernetes_scale_worker` add `lan_ip` to show node LAN IP.
* Resource `tencentcloud_kubernetes_cluster_attachment` add `state` to show node state.
* Resource `tencentcloud_clb_rule` support certificate modifying.
* Data Source `tencentcloud_clb_instances` add `internet_charge_type`, `internet_bandwidth_max_out`.
* Data Source `tencentcloud_clb_rules` add `http2_switch`.

BUG FIXES:

* Resource: `tencentcloud_clb_attachment` fix bug that attach more than 20 targets will failed.

## 1.53.4 (February 08, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_scale_worker` add `data_disk`, `docker_graph_path` to support advanced instance
  setting.
* Resource `tencentcloud_instance` add tags to the disks created with the instance.

BUG FIXES:

* Resource: `tencentcloud_kubernetes_cluster_attachment` fix bug that only one extra argument set successfully.
* Resource: `tencentcloud_as_scaling_policy` fix bug that missing required parameters error happened when update metric
  parameters.

## 1.53.3 (February 02, 2021)

ENHANCEMENTS:

* Data Source `tencentcloud_cbs_storages` add `throughput_performance` to support adding extra performance to the cbs
  resources.
* Resource `tencentcloud_kubernetes_cluster_attachment` add `hostname` to support setting hostname with the attached
  instance.

## 1.53.2 (February 01, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_cbs_storage` add `throughput_performance` to support adding extra performance to the cbs
  resources.

BUG FIXES:

* Resource: `tencentcloud_cos_bucket` fix bug that error happens when applying unsupported logging region.
* Resource: `tencentcloud_as_scaling_policy` fix bug that missing required parameters error happened when update metric
  parameters.

## 1.53.1 (January 23, 2021)

ENHANCEMENTS:

* Resource `tencentcloud_instance` add `throughput_performance` to support adding extra performance to the data disks.
* Resource `tencentcloud_kubernetes_cluster_attachment` add `file_system`, `auto_format_and_mount` and `mount_target` to
  support advanced instance setting.
* Resource `tencentcloud_kubernetes_node_pool` add `file_system`, `auto_format_and_mount` and `mount_target` to support
  advanced instance setting.
* Resource `tencentcloud_kubernetes_node_pool` add `scaling_mode` to support scaling mode setting.
* Resource `tencentcloud_kubernetes` support version upgrade.

BUG FIXES:

* Resource: `tencentcloud_gaap_http_rule` fix bug that exception happens when create more than one rule.

## 1.53.0 (January 15, 2021)

FEATURES:

* **New Resource**: `tencentcloud_ssl_pay_certificate` to support ssl pay certificate.

ENHANCEMENTS:

* Resource `tencentcloud_ccn` add `charge_type` to support billing mode setting.
* Resource `tencentcloud_ccn` add `bandwidth_limit_type` to support the speed limit type setting.
* Resource `tencentcloud_ccn_bandwidth_limit` add `dst_region` to support destination area restriction setting.
* Resource `tencentcloud_cdn_domain` add `range_origin_switch` to support range back to source configuration.
* Resource `tencentcloud_cdn_domain` add `rule_cache` to support advanced path cache configuration.
* Resource `tencentcloud_cdn_domain` add `request_header` to support request header configuration.
* Data Source `tencentcloud_ccn_instances` add `charge_type` to support billing mode.
* Data Source `tencentcloud_ccn_instances` add `bandwidth_limit_type` to support the speed limit type.
* Data Source `tencentcloud_ccn_bandwidth_limit` add `dst_region` to support destination area restriction.
* Data Source `tencentcloud_cdn_domains` add `range_origin_switch` to support range back to source configuration.
* Data Source `tencentcloud_cdn_domains` add `rule_cache` to support advanced path cache configuration.
* Data Source `tencentcloud_cdn_domains` add `request_header` to support request header configuration.

## 1.52.0 (December 28, 2020)

FEATURES:

* **New Resource**: `tencentcloud_kubernetes_node_pool` to support node management.

DEPRECATED:

* Resource: `tencentcloud_kubernetes_as_scaling_group` replaced by `tencentcloud_kubernetes_node_pool`.

## 1.51.1 (December 22, 2020)

ENHANCEMENTS:

* Resource `tencentcloud_kubernetes_cluster_attachment` add `extra_args` to support node extra arguments setting.
* Resource `tencentcloud_cos_bucket` add `log_enbale`, `log_target_bucket` and `log_prefix` to support log status
  setting.

## 1.51.0 (December 15, 2020)

FEATURES:

* **New Resource**: `tencentcloud_tcr_vpc_attachment`
* **New Data Source**: `tencentcloud_tcr_vpc_attachments`

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` support `name`, `project_id` and `description` modification.
* Doc: optimize document.

## 1.50.0 (December 08, 2020)

FEATURES:

* **New Resource**: `tencentcloud_address_template`
* **New Resource**: `tencentcloud_address_template_group`
* **New Resource**: `tencentcloud_protocol_template`
* **New Resource**: `tencentcloud_protocol_template_group`
* **New Data Source**: `tencentcloud_address_templates`
* **New Data Source**: `tencentcloud_address_template_groups`
* **New Data Source**: `tencentcloud_protocol_templates`
* **New Data Source**: `tencentcloud_protocol_template_groups`

ENHANCEMENTS:

* Resource `tencentcloud_sercurity_group_rule` add `address_template` and `protocol_template` to support building new
  security group rule with resource `tencentcloud_address_template` and `tencentcloud_protocol_template`.
* Doc: optimize document directory.

BUG FIXES:

* Resource: `tencentcloud_cos_bucket` fix bucket name validator.

## 1.49.1 (December 01, 2020)

ENHANCEMENTS:

* Doc: Update directory of document.

## 1.49.0 (November 27, 2020)

FEATURES:

* **New Resource**: `tencentcloud_tcr_instance`
* **New Resource**: `tencentcloud_tcr_token`
* **New Resource**: `tencentcloud_tcr_namespace`
* **New Resource**: `tencentcloud_tcr_repository`
* **New Data Source**: `tencentcloud_tcr_instances`
* **New Data Source**: `tencentcloud_tcr_tokens`
* **New Data Source**: `tencentcloud_tcr_namespaces`
* **New Data Source**: `tencentcloud_tcr_repositories`
* **New Resource**: `tencentcloud_cos_bucket_policy`

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_as_scaling_group` support `max_size` and `min_size` modification.

## 1.48.0 (November 20, 2020)

FEATURES:

* **New Resource**: `tencentcloud_sqlserver_basic_instance`
* **New Data Source**: `tencentcloud_sqlserver_basic_instances`

ENHANCEMENTS:

* Resource: `tencentcloud_clb_listener` support configure HTTP health check for TCP
  listener([#539](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/539)).
* Resource: `tencentcloud_clb_listener` add computed argument `target_type`.
* Data Source: `tencentcloud_clb_listeners` support getting HTTP health check config for TCP listener.

DEPRECATED:

* Resource: `tencentcloud_clb_target_group_attachment`: optional argument `targrt_group_id` is no longer supported,
  replace by `target_group_id`.

## 1.47.0 (November 13, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_clb_listener` support import.
* Resource: `tencentcloud_clb_listener` add computed argument `listener_id`.
* Resource: `tencentcloud_clb_listener_rule` support import.
* Resource: `tencentcloud_cdn_domain` add example that use COS bucket url as origin.
* Resource: `tencentcloud_sqlserver_instance` add new argument `tags`.
* Resource: `tencentcloud_sqlserver_readonly_instance` add new argument `tags`.
* Resource: `tencentcloud_elasticsearch_instance` support `node_type` and `disk_size` modification.
* Data Source: `tencentcloud_instance_types` add argument `exclude_sold_out` to support filtering sold out instance
  types.
* Data Source: `tencentcloud_sqlserver_instances` add new argument `tags`.
* Data Source: `tencentcloud_instance_types` add argument `exclude_sold_out` to support filtering sold out instance
  types.

BUG FIXES:

* Resource: `tencentcloud_elasticsearch_instance` fix inconsistent bug.
* Resource: `tencentcloud_redis_instance` fix incorrect number when updating `mem_size`.
* Data Source: `tencentcloud_redis_instances` fix incorrect number for `mem_size`.

## 1.46.4 (November 6, 2020)

BUG FIXES:

* Resource: `tencentcloud_kubernetes_cluster` fix force replacement when updating `docker_graph_path`.

## 1.46.3 (November 6, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add more values with argument `cluster_os` to support linux OS system.

## 1.46.2 (November 5, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add new argument `kube_config`.
* Resource: `tencentcloud_kubernetes_cluster` add value `tlinux2.4x86_64` with argument `cluster_os` to support linux OS
  system.
* Resource: `tencentcloud_kubernetes_cluster` add new argument `mount_target` to support set disk mount path.
* Resource: `tencentcloud_kubernetes_cluster` add new argument `docker_graph_path` to support set docker graph path.
* Resource: `tencentcloud_clb_redirection` add new argument `delete_all_auto_rewrite` to delete all auto-associated
  redirection when destroying the resource.
* Resource: `tencentcloud_kubernetes_scale_worker` add new argument `labels` to support scale worker labels.
* Data Source: `tencentcloud_kubernetes_clusters` add new argument `kube_config`.
* Data Source: `tencentcloud_availability_regions` support getting local region info by setting argument `name` with
  value `default`.
* Docs: update argument description.

BUG FIXES:

* Resource: `tencentcloud_clb_redirection` fix inconsistent bug when creating more than one auto redirection.
* Resource: `tencentcloud_redis_instance` fix updating issue when redis `type_id` is set `5`.

## 1.46.1 (October 29, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_cos_bucket` add new argument `cos_bucket_url`.
* Resource: `tencentcloud_nat_gateway` add new argument `tags`.
* Resource: `tencentcloud_postgresql_instance` add new argument `tags`.
* Data Source: `tencentcloud_cos_buckets` add new argument `cos_bucket_url`.
* Data Source: `tencentcloud_nat_gateways` add new argument `tags`.
* Data Source: `tencentcloud_postgresql_instances` add new argument `tags`.

## 1.46.0 (October 26, 2020)

FEATURES:

* **New Resource**: `tencentcloud_api_gateway_api`
* **New Resource**: `tencentcloud_api_gateway_service`
* **New Resource**: `tencentcloud_api_gateway_custom_domain`
* **New Resource**: `tencentcloud_api_gateway_usage_plan`
* **New Resource**: `tencentcloud_api_gateway_usage_plan_attachment`
* **New Resource**: `tencentcloud_api_gateway_ip_strategy`
* **New Resource**: `tencentcloud_api_gateway_strategy_attachment`
* **New Resource**: `tencentcloud_api_gateway_api_key`
* **New Resource**: `tencentcloud_api_gateway_api_key_attachment`
* **New Resource**: `tencentcloud_api_gateway_service_release`
* **New Data Source**: `tencentcloud_api_gateway_apis`
* **New Data Source**: `tencentcloud_api_gateway_services`
* **New Data Source**: `tencentcloud_api_gateway_throttling_apis`
* **New Data Source**: `tencentcloud_api_gateway_throttling_services`
* **New Data Source**: `tencentcloud_api_gateway_usage_plans`
* **New Data Source**: `tencentcloud_api_gateway_ip_strategies`
* **New Data Source**: `tencentcloud_api_gateway_customer_domains`
* **New Data Source**: `tencentcloud_api_gateway_usage_plan_environments`
* **New Data Source**: `tencentcloud_api_gateway_api_keys`

## 1.45.3 (October 21, 2020)

BUG FIXES:

* Resource: `tencentcloud_sqlserver_instance` Fix the error of releasing associated resources when destroying sqlserver
  postpaid instance.
* Resource: `tencentcloud_sqlserver_readonly_instance` Fix the bug that the instance cannot be recycled when destroying
  sqlserver postpaid instance.
* Resource: `tencentcloud_clb_instance` fix force new when updating tags.
* Resource: `tencentcloud_redis_backup_config` fix doc issues.
* Resource: `tencentcloud_instance` fix `keep_image_login` force new issue when updating terraform version.
* Resource: `tencentcloud_clb_instance` fix tag creation bug.

## 1.45.2 (October 19, 2020)

BUG FIXES:

* Resource: `tencentcloud_mysql_instance` fix creating prepaid instance error.

## 1.45.1 (October 16, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_clb_target_group_instance_attachment` update doc.
* Resource: `tencentcloud_clb_target_group_attachment` update doc.

## 1.45.0 (October 15, 2020)

FEATURES:

* **New Resource**: `tencentcloud_clb_target_group_attachment`
* **New Resource**: `tencentcloud_clb_target_group`
* **New Resource**: `tencentcloud_clb_target_group_instance_attachment`
* **New Resource**: `tencentcloud_sqlserver_publish_subscribe`
* **New Resource**: `tencentcloud_vod_adaptive_dynamic_streaming_template`
* **New Resource**: `tencentcloud_vod_procedure_template`
* **New Resource**: `tencentcloud_vod_snapshot_by_time_offset_template`
* **New Resource**: `tencentcloud_vod_image_sprite_template`
* **New Resource**: `tencentcloud_vod_super_player_config`
* **New Data Source**: `tencentcloud_clb_target_groups`
* **New Data Source**: `tencentcloud_sqlserver_publish_subscribes`
* **New Data Source**: `tencentcloud_vod_adaptive_dynamic_streaming_templates`
* **New Data Source**: `tencentcloud_vod_image_sprite_templates`
* **New Data Source**: `tencentcloud_vod_procedure_templates`
* **New Data Source**: `tencentcloud_vod_snapshot_by_time_offset_templates`
* **New Data Source**: `tencentcloud_vod_super_player_configs`

ENHANCEMENTS:

* Resource: `tencentcloud_clb_listener_rule` add new argument `target_type` to support backend target type with rule.
* Resource: `tencentcloud_mysql_instance` modify argument `engine_version` to support mysql 8.0.
* Resource: `tencentcloud_clb_listener_rule` add new argument `forward_type` to support backend
  protocol([#522](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/522)).
* Resource: `tencentcloud_instance` add new argument `keep_image_login` to support keeping image login.
* Resource: `tencentcloud_kubernetes_cluster` add new argument `extra_args` to support Kubelet.
* Resource: `tencentcloud_kubernetes_scale_worker` add new argument `extra_args` to support Kubelet.
* Resource: `tencentcloud_kubernetes_as_scaling_group` add new argument `extra_args` to support Kubelet.

## 1.44.0 (September 25, 2020)

FEATURES:

* **New Resource**: `tencentcloud_cynosdb_cluster`
* **New Resource**: `tencentcloud_cynosdb_readonly_instance`.
* **New Data Source**: `tencentcloud_cynosdb_clusters`
* **New Data Source**: `tencentcloud_cynosdb_readonly_instances`.

ENHANCEMENTS:

* Resource: `tencentcloud_mongodb_standby_instance` change example type to `POSTPAID`.
* Resource: `tencentcloud_instance` add new argument `encrypt` to support data disk with encrypt.
* Resource: `tencentcloud_elasticsearch` add new argument `encrypt` to support disk with encrypt.
* Resource: `tencentcloud_kubernetes_cluster` add new argument `cam_role_name` to support authorization with instances.

## 1.43.0 (September 18, 2020)

FEATURES:

* **New Resource**: `tencentcloud_image`
* **New Resource**: `tencentcloud_audit`
* **New Data Source**: `tencentcloud_audits`
* **New Data Source**: `tencentcloud_audit_cos_regions`
* **New Data Source**: `tencentcloud_audit_key_alias`

ENHANCEMENTS:

* Resource: `tencentcloud_instance` add new argument `data_disk_snapshot_id` to support data disk
  with `SnapshotId`([#469](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/469))
* Data Source: `tencentcloud_instances` support filter by tags.

## 1.42.2 (September 14, 2020)

BUG FIXES:

* Resource: `tencentcloud_instance` fix `key_name` update
  error([#515](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/515)).

## 1.42.1 (September 10, 2020)

BUG FIXES:

* Resource: `tencentcloud_mongodb_instance` Fix the error of releasing associated resources when destroying mongodb
  postpaid instance.
* Resource: `tencentcloud_mongodb_sharding_instance` Fix the error of releasing associated resources when destroying
  mongodb postpaid sharding instance.
* Resource: `tencentcloud_mongodb_standby_instance` Fix the error of releasing associated resources when destroying
  mongodb postpaid standby instance.

## 1.42.0 (September 8, 2020)

FEATURES:

* **New Resource**: `tencentcloud_ckafka_topic`
* **New Data Source**: `tencentcloud_ckafka_topics`

ENHANCEMENTS:

* Doc: optimize document directory.
* Resource: `tencentcloud_mongodb_instance`, `tencentcloud_mongodb_sharding_instance`
  and `tencentcloud_mongodb_standby_instance` remove system reserved tag `project`.

## 1.41.3 (September 3, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_vpc_acl_attachment` perfect example field `subnet_ids`
  to `subnet_id`([#505](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/505)).
* Resource: `tencentcloud_cbs_storage_attachment` support import.
* Resource: `tencentcloud_eip_association` support import.
* Resource: `tencentcloud_route_table_entry` support import.
* Resource: `tencentcloud_acl_attachment` support import.

## 1.41.2 (August 28, 2020)

BUG FIXES:

* Resource: `tencentcloud_vpn_connection` fix `security_group_policy` update issue when apply repeatedly.
* Resource: `tencentcloud_vpn_connection` fix inconsistent state when deleted on console.

## 1.41.1 (August 27, 2020)

BUG FIXES:

* Resource: `tencentcloud_vpn_gateway` fix force new issue when apply repeatedly.
* Resource: `tencentcloud_vpn_connection` fix force new issue when apply repeatedly.
* Resource: `tencentcloud_instance` support for adjusting `internet_max_bandwidth_out` without forceNew when
  attribute `internet_charge_type` within `TRAFFIC_POSTPAID_BY_HOUR`,`BANDWIDTH_POSTPAID_BY_HOUR`
  ,`BANDWIDTH_PACKAGE` ([#498](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/498)).

## 1.41.0 (August 17, 2020)

FEATURES:

* **New Resource**: `tencentcloud_sqlserver_instance`
* **New Resource**: `tencentcloud_sqlserver_readonly_instance`
* **New Resource**: `tencentcloud_sqlserver_db`
* **New Resource**: `tencentcloud_sqlserver_account`
* **New Resource**: `tencentcloud_sqlserver_db_account_attachment`
* **New Resource**: `tencentcloud_vpc_acl`
* **New Resource**: `tencentcloud_vpc_acl_attachment`
* **New Resource**: `tencentcloud_ckafka_acl`
* **New Resource**: `tencentcloud_ckafka_user`
* **New Data Source**: `tencentcloud_sqlserver_instance`
* **New Data Source**: `tencentcloud_sqlserver_readonly_groups`
* **New Data Source**: `tencentcloud_vpc_acls`
* **New Data Source**: `tencentcloud_ckafka_acls`
* **New Data Source**: `tencentcloud_ckafka_users`

DEPRECATED:

* Data Source: `tencentcloud_cdn_domains` optional argument `offset` is no longer supported.

ENHANCEMENTS:

* Resource: `tencentcloud_mongodb_instance`, `tencentcloud_mongodb_sharding_instance`
  and `tencentcloud_mongodb_standby_instance` remove spec update validation.

## 1.40.3 (August 11, 2020)

ENHANCEMENTS:

* Data Source: `tencentcloud_kubernetes_clusters`add new attributes `cluster_as_enabled`,`node_name_type`
  ,`cluster_extra_args`,`network_type`,`is_non_static_ip_mode`,`kube_proxy_mode`,`service_cidr`,`eni_subnet_ids`
  ,`claim_expired_seconds` and `deletion_protection`.

BUG FIXES:

* Resource: `tencentcloud_vpn_gateway` fix creation of instance when `vpc_id` is specified.
* Resource: `tencentcloud_vpn_connection` fix creation of instance when `vpc_id` is specified.
* Resource: `tencentcloud_instance` fix `internet_charge_type` inconsistency when public ip is not allocated.

## 1.40.2 (August 08, 2020)

BUG FIXES:

* Resource: `tencentcloud_instance` fix accidentally fail to delete prepaid
  instance ([#485](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/485)).

## 1.40.1 (August 05, 2020)

BUG FIXES:

* Resource: `tencentcloud_vpn_connection` fix mulit `security_group_policy` is not
  supported ([#487](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/487)).

## 1.40.0 (July 31, 2020)

FEATURES:

* **New Resource**: `tencentcloud_mongodb_standby_instance`

ENHANCEMENTS:

* Resource: `tencentcloud_gaap_http_rule` argument `realservers` now is optional.
* Resource: `tencentcloud_kubernetes_cluster` supports multiple `availability_zone`.
* Data Source: `tencentcloud_mongodb_instances` add new argument `charge_type` and `auto_renew_flag` to support prepaid
  type.
* Resource: `tencentcloud_mongodb_instance` supports prepaid type, new mongodb SDK version `2019-07-25` and standby
  instance.
* Resource: `tencentcloud_mongodb_sharding_instance` supports prepaid type, new mongodb SDK version `2019-07-25` and
  standby instance.
* Resource: `tencentcloud_security_group_lite_rule` refine update process and doc.

BUG FIXES:

* Resource: `tencentcloud_instance` fix set `key_name` error.

## 1.39.0 (July 18, 2020)

ENHANCEMENTS:

* upgrade terraform 0.13
* update readme to new repository

## 1.38.3 (July 13, 2020)

ENHANCEMENTS:

* Data Source: `tencentcloud_images` supports list of snapshots.
* Resource: `tencentcloud_kubernetes_cluster_attachment` add new argument `worker_config` to support config with
  existing instances.
* Resource: `tencentcloud_ccn` add new argument `tags` to support tags settings.
* Resource: `tencentcloud_cfs_file_system` add new argument `tags` to support tags settings.

BUG FIXES:

* Resource: `tencentcloud_gaap_layer4_listener` fix error InvalidParameter when destroy resource.
* Resource: `tencentcloud_gaap_layer7_listener` fix error InvalidParameter when destroy resource.
* Resource: `tencentcloud_cdn_domain` fix incorrect setting `server_certificate_config`, `client_certificate_config`
  caused the program to crash.

## 1.38.2 (July 03, 2020)

BUG FIXES:

* Resource: `tencentcloud_instance` fix `allocate_public_ip` inconsistency when eip is attached to the cvm.
* Resource: `tencentcloud_mysql_instance` fix auto-forcenew on `charge_type` and `pay_type` when upgrading terraform
  version. ([#459](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/pull/459)).

## 1.38.1 (June 30, 2020)

BUG FIXES:

* Resource: `tencentcloud_cos_bucket` fix creation failure.

## 1.38.0 (June 29, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_cdn_domains`

BUG FIXES:

* Resource: `tencentcloud_gaap_http_domain` fix a condition for setting client certificate
  ids([#454](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/pull/454)).

## 1.37.0 (June 23, 2020)

FEATURES:

* **New Resource**: `tencentcloud_postgresql_instance`
* **New Data Source**: `tencentcloud_postgresql_instances`
* **New Data Source**: `tencentcloud_postgresql_speccodes`
* **New Data Source**: `tencentcloud_sqlserver_zone_config`

ENHANCEMENTS:

* Resource: `tencentcloud_mongodb_instance` support more machine type.

## 1.36.1 (June 12, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add new argument `labels`.
* Resource: `tencentcloud_kubernetes_as_scaling_group` add new argument `labels`.
* Resource: `tencentcloud_cos_bucket` add new arguments `encryption_algorithm` and `versioning_enable`.

## 1.36.0 (June 08, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_availability_regions`

ENHANCEMENTS:

* Data Source: `tencentcloud_redis_instances` add new argument `charge_type` to support prepaid type.
* Resource: `tencentcloud_redis_instance` add new argument `charge_type`, `prepaid_period` and `force_delete` to support
  prepaid type.
* Resource: `tencentcloud_mysql_instance` add new argument `force_delete` to support soft deletion.
* Resource: `tencentcloud_mysql_readonly_instance` add new argument `force_delete` to support soft deletion.

BUG FIXES:

* Resource: `tencentcloud_instance` fix `allocate_public_ip` inconsistency when eip is attached to the cvm.

DEPRECATED:

* Data Source: `tencentcloud_mysql_instances`: optional argument `pay_type` is no longer supported, replace
  by `charge_type`.
* Resource: `tencentcloud_mysql_instance`: optional arguments `pay_type` and `period` are no longer supported, replace
  by `charge_type` and `prepaid_period`.
* Resource: `tencentcloud_mysql_readonly_instance`: optional arguments `pay_type` and `period` are no longer supported,
  replace by `charge_type` and `prepaid_period`.
* Resource: `tencentcloud_tcaplus_group` replace by `tencentcloud_tcaplus_tablegroup`
* Data Source: `tencentcloud_tcaplus_groups` replace by `tencentcloud_tcaplus_tablegroups`
* Resource: `tencentcloud_tcaplus_tablegroup`,`tencentcloud_tcaplus_idl` and `tencentcloud_tcaplus_table`
  arguments `group_id`/`group_name`  replace by `tablegroup_id`/`tablegroup_name`
* Data Source: `tencentcloud_tcaplus_groups`,`tencentcloud_tcaplus_idls` and `tencentcloud_tcaplus_tables`
  arguments `group_id`/`group_name`  replace by `tablegroup_id`/`tablegroup_name`

## 1.35.1 (June 02, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_as_scaling_config`, `tencentcloud_eip` and `tencentcloud_kubernetes_cluster` remove the
  validate function of `internet_max_bandwidth_out`.
* Resource: `tencentcloud_vpn_gateway` update available value of `bandwidth`.

## 1.35.0 (June 01, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_elasticsearch_instances`
* **New Resource**: `tencentcloud_elasticsearch_instance`

## 1.34.0 (May 28, 2020)

ENHANCEMENTS:

* upgrade terraform-plugin-sdk

## 1.33.2 (May 25, 2020)

DEPRECATED:

* Data Source: `tencentcloud_tcaplus_applications` replace by `tencentcloud_tcaplus_clusters`,optional
  arguments `app_id` and `app_name` are no longer supported, replace by `cluster_id` and `cluster_name`
* Data Source: `tencentcloud_tcaplus_zones` replace by `tencentcloud_tcaplus_groups`,optional arguments `app_id`
  ,`zone_id` and `zone_name` are no longer supported, replace by `cluster_id`,`group_id` and `cluster_name`
* Data Source: `tencentcloud_tcaplus_tables` optional arguments `app_id` and `zone_id` are no longer supported, replace
  by `cluster_id` and `group_id`
* Data Source: `tencentcloud_tcaplus_idls`: optional argument `app_id` is no longer supported, replace by `cluster_id`.
* Resource: `tencentcloud_tcaplus_application` replace by `tencentcloud_tcaplus_cluster`,input argument `app_name` is no
  longer supported, replace by `cluster_name`
* Resource: `tencentcloud_tcaplus_zone` replace by `tencentcloud_tcaplus_group`, input arguments `app_id`
  and `zone_name` are no longer supported, replace by `cluster_id` and `group_name`
* Resource: `tencentcloud_tcaplus_idl` input arguments `app_id` and `zone_id` are no longer supported, replace
  by `cluster_id` and `group_id`
* Resource: `tencentcloud_tcaplus_table` input arguments `app_id`and `zone_id` are no longer supported, replace
  by `cluster_id` and `group_id`
* Resource: `tencentcloud_redis_instance`: optional argument `type` is no longer supported, replace by `type_id`.
* Data Source: `tencentcloud_redis_instances`: output argument `type` is no longer supported, replace by `type_id`.
* Data Source: `tencentcloud_redis_zone_config`: output argument `type` is no longer supported, replace by `type_id`.

## 1.33.1 (May 22, 2020)

ENHANCEMENTS:

* Data Source: `tencentcloud_redis_instances` add new argument `type_id`, `redis_shard_num`, `redis_replicas_num`
* Data Source: `tencentcloud_redis_zone_config` add output argument `type_id` and new output argument `type_id`
  , `redis_shard_nums`, `redis_replicas_nums`
* Data Source: `tencentcloud_ccn_instances` add new type `VPNGW` for field `instance_type`
* Data Source: `tencentcloud_vpn_gateways` add new type `CCN` for field `type`
* Resource: `tencentcloud_redis_instance` add new argument `type_id`, `redis_shard_num`, `redis_replicas_num`
* Resource: `tencentcloud_ccn_attachment` add new type `CNN_INSTANCE_TYPE_VPNGW` for field `instance_type`
* Resource: `tencentcloud_vpn_gateway` add new type `CCN` for field `type`

BUG FIXES:

* Resource: `tencentcloud_cdn_domain` fix `https_config` inconsistency after
  apply([#413](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/413)).

DEPRECATED:

* Resource: `tencentcloud_redis_instance`: optional argument `type` is no longer supported, replace by `type_id`.
* Data Source: `tencentcloud_redis_instances`: output argument `type` is no longer supported, replace by `type_id`.
* Data Source: `tencentcloud_redis_zone_config`: output argument `type` is no longer supported, replace by `type_id`.

## 1.33.0 (May 18, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_monitor_policy_conditions`
* **New Data Source**: `tencentcloud_monitor_data`
* **New Data Source**: `tencentcloud_monitor_product_event`
* **New Data Source**: `tencentcloud_monitor_binding_objects`
* **New Data Source**: `tencentcloud_monitor_policy_groups`
* **New Data Source**: `tencentcloud_monitor_product_namespace`
* **New Resource**: `tencentcloud_monitor_policy_group`
* **New Resource**: `tencentcloud_monitor_binding_object`
* **New Resource**: `tencentcloud_monitor_binding_receiver`

ENHANCEMENTS:

* Data Source: `tencentcloud_instances` add new output argument `instance_charge_type_prepaid_renew_flag`.
* Data Source: `tencentcloud_cbs_storages` add new output argument `prepaid_renew_flag`.
* Data Source: `tencentcloud_cbs_storages` add new output argument `charge_type`.
* Resource: `tencentcloud_instance` support update with argument `instance_charge_type_prepaid_renew_flag`.
* Resource: `tencentcloud_cbs_storage` add new argument `force_delete`.
* Resource: `tencentcloud_cbs_storage` add new argument `charge_type`.
* Resource: `tencentcloud_cbs_storage` add new argument `prepaid_renew_flag`.
* Resource: `tencentcloud_cdn_domain` add new
  argument `full_url_cache`([#405](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/405)).

DEPRECATED:

* Resource: `tencentcloud_cbs_storage`: optional argument `period` is no longer supported.

## 1.32.1 (April 30, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_ccn_attachment` add new argument `ccn_uin`.
* Resource: `tencentcloud_instance` add new argument `force_delete`.

BUG FIXES:

* Resource: `tencentcloud_scf_function` fix update `zip_file`.

## 1.32.0 (April 20, 2020)

FEATURES:

* **New
  Resource**: `tencentcloud_kubernetes_cluster_attachment`([#285](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/285))
  .

ENHANCEMENTS:

* Resource: `tencentcloud_cdn_domain` add new
  attribute `cname`([#395](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/395)).

BUG FIXES:

* Resource: `tencentcloud_cos_bucket_object` mark the object as destroyed when the object not exist.

## 1.31.2 (April 17, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_cbs_storage` support modify `tags`.

## 1.31.1 (April 14, 2020)

BUG FIXES:

* Resource: `tencentcloud_keypair` fix bug when trying to destroy resources containing CVM and key
  pair([#375](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/375)).
* Resource: `tencentcloud_clb_attachment` fix bug when trying to destroy multiple attachments in the array.
* Resource: `tencentcloud_cam_group_membership` fix bug when trying to destroy multiple users in the array.

ENHANCEMENTS:

* Resource: `tencentcloud_mysql_account` add new
  argument `host`([#372](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/372)).
* Resource: `tencentcloud_mysql_account_privilege` add new
  argument `account_host`([#372](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/372)).
* Resource: `tencentcloud_mysql_privilege` add new
  argument `account_host`([#372](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/372)).
* Resource: `tencentcloud_mysql_readonly_instance` check master monitor data before
  create([#379](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/379)).
* Resource: `tencentcloud_tcaplus_application` remove the pull password from server.
* Resource: `tencentcloud_instance` support
  import `allocate_public_ip`([#382](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/382)).
* Resource: `tencentcloud_redis_instance` add two redis types.
* Data Source: `tencentcloud_vpc_instances` add new argument `cidr_block`
  ,`tag_key` ([#378](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/378)).
* Data Source: `tencentcloud_vpc_route_tables` add new argument `tag_key`,`vpc_id`
  ,`association_main` ([#378](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/378)).
* Data Source: `tencentcloud_vpc_subnets` add new argument `cidr_block`,`tag_key`
  ,`is_remote_vpc_snat` ([#378](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/378)).
* Data Source: `tencentcloud_mysql_zone_config` and `tencentcloud_redis_zone_config` remove region check.

## 1.31.0 (April 07, 2020)

FEATURES:

* **New Resource**: `tencentcloud_cdn_domain`

ENHANCEMENTS:

* Data Source: `tencentcloud_cam_users` add new argument `user_id`.
* Resource: `tencentcloud_vpc` add retry logic.

BUG FIXES:

* Resource: `tencentcloud_instance` fix timeout error when modify password.

## 1.30.7 (March 31, 2020)

BUG FIXES:

* Resource: `tencentcloud_kubernetes_as_scaling_group` set a value to argument `key_ids` cause error .

## 1.30.6 (March 30, 2020)

ENHANCEMENTS:

* Resource: `tencentcloud_tcaplus_idl` add new argument `zone_id`.
* Resource: `tencentcloud_cam_user` add new argument `force_delete`
  .([#354](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/354))
* Data Source: `tencentcloud_vpc_subnets` add new argument `vpc_id`.

## 1.30.5 (March 19, 2020)

BUG FIXES:

* Resource: `tencentcloud_key_pair` will be replaced when `public_key` contains comment.
* Resource: `tencentcloud_scf_function` upload local file error.

ENHANCEMENTS:

* Resource: `tencentcloud_scf_function` runtime support nodejs8.9 and nodejs10.15.

## 1.30.4 (March 10, 2020)

BUG FIXES:

* Resource: `tencentcloud_cam_policy` fix read nil issue when the resource is not
  exist.([#344](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/#344)).
* Resource: `tencentcloud_key_pair` will be replaced when the end of `public_key` contains
  spaces([#343](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/343)).
* Resource: `tencentcloud_scf_function` fix trigger does not support cos_region.

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add new attributes `cluster_os_type`,`cluster_internet`,`cluster_intranet`
  ,`managed_cluster_internet_security_policies` and `cluster_intranet_subnet_id`.

## 1.30.3 (February 24, 2020)

BUG FIXES:

* Resource: `tencentcloud_instance` fix that classic network does not
  support([#339](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/339)).

## 1.30.2 (February 17, 2020)

ENHANCEMENTS:

* Data Source: `tencentcloud_cam_policies` add new attribute `policy_id`.
* Data Source: `tencentcloud_cam_groups` add new attribute `group_id`.

## 1.30.1 (January 21, 2020)

BUG FIXES:

* Resource: `tencentcloud_dnat` fix `elastic_port` and `internal_port` type error.
* Resource: `tencentcloud_vpn_gateway` fix `state` type error.
* Resource: `tencentcloud_dayu_ddos_policy` fix that `white_ips` and `black_ips` can not be updated.
* Resource: `tencentcloud_dayu_l4_rule` fix that rule parameters can not be updated.

ENHANCEMENTS:

* Data Source: `tencentcloud_key_pairs` support regular expression search by name.

## 1.30.0 (January 14, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_dayu_cc_http_policies`
* **New Data Source**: `tencentcloud_dayu_cc_https_policies`
* **New Data Source**: `tencentcloud_dayu_ddos_policies`
* **New Data Source**: `tencentcloud_dayu_ddos_policy_attachments`
* **New Data Source**: `tencentcloud_dayu_ddos_policy_cases`
* **New Data Source**: `tencentcloud_dayu_l4_rules`
* **New Data Source**: `tencentcloud_dayu_l7_rules`
* **New Resource**: `tencentcloud_dayu_cc_http_policy`
* **New Resource**: `tencentcloud_dayu_cc_https_policy`
* **New Resource**: `tencentcloud_dayu_ddos_policy`
* **New Resource**: `tencentcloud_dayu_ddos_policy_attachment`
* **New Resource**: `tencentcloud_dayu_ddos_policy_case`
* **New Resource**: `tencentcloud_dayu_l4_rule`
* **New Resource**: `tencentcloud_dayu_l7_rule`

BUG FIXES:

* gaap: optimize gaap describe: when describe resource by id but get more than 1 resources, return error directly
  instead of using the first result
* Resource: `tencentcloud_eni_attachment` fix detach may failed.
* Resource: `tencentcloud_instance` remove the tag that be added by as attachment
  automatically([#300](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/300)).
* Resource: `tencentcloud_clb_listener` fix `sni_switch` type
  error([#297](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/297)).
* Resource: `tencentcloud_vpn_gateway` shows argument `prepaid_renew_flag` has changed when applied
  again([#298](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/298)).
* Resource: `tencentcloud_clb_instance` fix the bug that instance id is not set in state
  file([#303](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/303)).
* Resource: `tencentcloud_vpn_gateway` that is postpaid charge type cannot be deleted
  normally([#312](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/312)).
* Resource: `tencentcloud_vpn_gateway` add `InternalError` SDK error to triggering the retry process.
* Resource: `tencentcloud_vpn_gateway` fix read nil issue when the resource is not exist.
* Resource: `tencentcloud_clb_listener_rule` fix unclear error message of SSL type error.
* Resource: `tencentcloud_ha_vip_attachment` fix read nil issue when the resource is not exist.
* Data Source: `tencentcloud_security_group` fix `project_id` type error.
* Data Source: `tencentcloud_security_groups` fix `project_id` filter not
  works([#303](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/314)).

## 1.29.0 (January 06, 2020)

FEATURES:

* **New Data Source**: `tencentcloud_gaap_domain_error_pages`
* **New Resource**: `tencentcloud_gaap_domain_error_page`

ENHANCEMENTS:

* Data Source: `tencentcloud_vpc_instances` add new optional argument `is_default`.
* Data Source: `tencentcloud_vpc_subnets` add new optional argument `availability_zone`,`is_default`.

BUG FIXES:

* Resource: `tencentcloud_redis_instance` field security_groups are id list, not name
  list([#291](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/291)).

## 1.28.0 (December 25, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_cbs_snapshot_policies`
* **New Resource**: `tencentcloud_cbs_snapshot_policy_attachment`

ENHANCEMENTS:

* doc: rewrite website index
* Resource: `tencentcloud_instance` support modifying instance
  type([#251](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/251)).
* Resource: `tencentcloud_gaap_http_domain` add new optional argument `realserver_certificate_ids`.
* Data Source: `tencentcloud_gaap_http_domains` add new output argument `realserver_certificate_ids`.

DEPRECATED:

* Resource: `tencentcloud_gaap_http_domain`: optional argument `realserver_certificate_id` is no longer supported.
* Data Source: `tencentcloud_gaap_http_domains`: output argument `realserver_certificate_id` is no longer supported.

## 1.27.0 (December 17, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_tcaplus_applications`
* **New Data Source**: `tencentcloud_tcaplus_zones`
* **New Data Source**: `tencentcloud_tcaplus_tables`
* **New Data Source**: `tencentcloud_tcaplus_idls`
* **New Resource**: `tencentcloud_tcaplus_application`
* **New Resource**: `tencentcloud_tcaplus_zone`
* **New Resource**: `tencentcloud_tcaplus_idl`
* **New Resource**: `tencentcloud_tcaplus_table`

ENHANCEMENTS:

* Resource: `tencentcloud_mongodb_instance` support more instance
  type([#241](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/241)).
* Resource: `tencentcloud_kubernetes_cluster` support more instance
  type([#237](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/237)).

BUG FIXES:

* Fix bug that resource `tencentcloud_instance` delete error when instance launch failed.
* Fix bug that resource `tencentcloud_security_group` read error when response is InternalError.
* Fix bug that the type of `cluster_type` is wrong in data
  source `tencentcloud_mongodb_instances`([#242](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/242))
  .
* Fix bug that resource `tencentcloud_eip` unattach
  error([#233](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/233)).
* Fix bug that terraform read nil attachment resource when the attached resource of attachment resource is removed of
  resource CLB and CAM.
* Fix doc example error of resource `tencentcloud_nat_gateway`.

DEPRECATED:

* Resource: `tencentcloud_eip`: optional argument `applicable_for_clb` is no longer supported.

## 1.26.0 (December 09, 2019)

FEATURES:

* **New
  Resource**: `tencentcloud_mysql_privilege`([#223](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/223))
  .
* **New
  Resource**: `tencentcloud_kubernetes_as_scaling_group`([#202](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/202))
  .

ENHANCEMENTS:

* Resource: `tencentcloud_gaap_layer4_listener` support import.
* Resource: `tencentcloud_gaap_http_rule` support import.
* Resource: `tencentcloud_gaap_security_rule` support import.
* Resource: `tencentcloud_gaap_http_domain` add new optional argument `client_certificate_ids`.
* Resource: `tencentcloud_gaap_layer7_listener` add new optional argument `client_certificate_ids`.
* Data Source: `tencentcloud_gaap_http_domains` add new output argument `client_certificate_ids`.
* Data Source: `tencentcloud_gaap_layer7_listeners` add new output argument `client_certificate_ids`.

DEPRECATED:

* Resource: `tencentcloud_gaap_http_domain`: optional argument `client_certificate_id` is no longer supported.
* Resource: `tencentcloud_gaap_layer7_listener`: optional argument `client_certificate_id` is no longer supported.
* Resource: `tencentcloud_mysql_account_privilege` replaced by `tencentcloud_mysql_privilege`.
* Data Source: `tencentcloud_gaap_http_domains`: output argument `client_certificate_id` is no longer supported.
* Data Source: `tencentcloud_gaap_layer7_listeners`: output argument `client_certificate_id` is no longer supported.

BUG FIXES:

* Fix bug that resource `tencentcloud_clb_listener` 's
  unchangeable `health_check_switch`([#235](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/235))
  .
* Fix bug that resource `tencentcloud_clb_instance` read nil and report error.
* Fix example errors of resource `tencentcloud_cbs_snapshot_policy` and data source `tencentcloud_dnats`.

## 1.25.2 (December 04, 2019)

BUG FIXES:

* Fixed bug that the validator of cvm instance type is incorrect.

## 1.25.1 (December 03, 2019)

ENHANCEMENTS:

* Optimized error message of validators.

BUG FIXES:

* Fixed bug that the type of `state` is incorrect in data
  source `tencentcloud_nat_gateways`([#226](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/226))
  .
* Fixed bug that the value of `cluster_max_pod_num` is incorrect in
  resource `tencentcloud_kubernetes_cluster`([#228](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/228))
  .

## 1.25.0 (December 02, 2019)

ENHANCEMENTS:

* Resource: `tencentcloud_instance` support `SPOTPAID` instance. Thanks to
  @LipingMao ([#209](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/209)).
* Resource: `tencentcloud_vpn_gateway` add argument `prepaid_renew_flag` and `prepaid_period` to support prepaid VPN
  gateway instance creation.

BUG FIXES:

* Fixed bugs that update operations on `tencentcloud_cam_policy` do not work.
* Fixed bugs that filters on `tencentcloud_cam_users` do not work.

DEPRECATED:

* Data Source: `tencentcloud_cam_user_policy_attachments`:`policy_type` is no longer supported.
* Data Source: `tencentcloud_cam_group_policy_attachments`:`policy_type` is no longer supported.

## 1.24.1 (November 26, 2019)

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` add support for `PREPAID` instance type. Thanks to
  @woodylic ([#204](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/204)).
* Resource: `tencentcloud_cos_bucket` add optional argument tags
* Data Source: `tencentcloud_cos_buckets` add optional argument tags

BUG FIXES:

* Fixed docs issues of `tencentcloud_nat_gateway`

## 1.24.0 (November 20, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_ha_vips`
* **New Data Source**: `tencentcloud_ha_vip_eip_attachments`
* **New Resource**: `tencentcloud_ha_vip`
* **New Resource**: `tencentcloud_ha_vip_eip_attachment`

ENHANCEMENTS:

* Resource: `tencentcloud_kubernetes_cluster` cluster_os add new support: `centos7.6x86_64`
  and `ubuntu18.04.1 LTSx86_64`
* Resource: `tencentcloud_nat_gateway` add computed argument `created_time`.

BUG FIXES:

* Fixed docs issues of CAM, DNAT and NAT_GATEWAY
* Fixed query issue that paged-query was not supported in data source `tencentcloud_dnats`
* Fixed query issue that filter `address_ip` was set incorrectly in data source `tencentcloud_eips`

## 1.23.0 (November 14, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_images`
* **New Data Source**: `tencentcloud_vpn_gateways`
* **New Data Source**: `tencentcloud_customer_gateways`
* **New Data Source**: `tencentcloud_vpn_connections`
* **New Resource**: `tencentcloud_vpn_gateway`
* **New Resource**: `tencentcloud_customer_gateway`
* **New Resource**: `tencentcloud_vpn_connection`
* **Provider TencentCloud**: add `security_token` argument

ENHANCEMENTS:

* All api calls now using api3.0
* Resource: `tencentcloud_eip` add optional argument `tags`.
* Data Source: `tencentcloud_eips` add optional argument `tags`.

BUG FIXES:

* Fixed docs of CAM

## 1.22.0 (November 05, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_cfs_file_systems`
* **New Data Source**: `tencentcloud_cfs_access_groups`
* **New Data Source**: `tencentcloud_cfs_access_rules`
* **New Data Source**: `tencentcloud_scf_functions`
* **New Data Source**: `tencentcloud_scf_namespaces`
* **New Data Source**: `tencentcloud_scf_logs`
* **New Resource**: `tencentcloud_cfs_file_system`
* **New Resource**: `tencentcloud_cfs_access_group`
* **New Resource**: `tencentcloud_cfs_access_rule`
* **New Resource**: `tencentcloud_scf_function`
* **New Resource**: `tencentcloud_scf_namespace`

## 1.21.2 (October 29, 2019)

BUG FIXES:

* Resource: `tencentcloud_gaap_realserver` add ip/domain exists check
* Resource: `tencentcloud_kubernetes_cluster` add error handling logic and optional argument `tags`.
* Resource: `tencentcloud_kubernetes_scale_worker` add error handling logic.
* Data Source: `tencentcloud_kubernetes_clusters` add optional argument `tags`.

## 1.21.1 (October 23, 2019)

ENHANCEMENTS:

* Updated golang to version 1.13.x

BUG FIXES:

* Fixed docs of CAM

## 1.21.0 (October 15, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_cam_users`
* **New Data Source**: `tencentcloud_cam_groups`
* **New Data Source**: `tencentcloud_cam_policies`
* **New Data Source**: `tencentcloud_cam_roles`
* **New Data Source**: `tencentcloud_cam_user_policy_attachments`
* **New Data Source**: `tencentcloud_cam_group_policy_attachments`
* **New Data Source**: `tencentcloud_cam_role_policy_attachments`
* **New Data Source**: `tencentcloud_cam_group_memberships`
* **New Data Source**: `tencentcloud_cam_saml_providers`
* **New Data Source**: `tencentcloud_reserved_instance_configs`
* **New Data Source**: `tencentcloud_reserved_instances`
* **New Resource**: `tencentcloud_cam_user`
* **New Resource**: `tencentcloud_cam_group`
* **New Resource**: `tencentcloud_cam_role`
* **New Resource**: `tencentcloud_cam_policy`
* **New Resource**: `tencentcloud_cam_user_policy_attachment`
* **New Resource**: `tencentcloud_cam_group_policy_attachment`
* **New Resource**: `tencentcloud_cam_role_policy_attachment`
* **New Resource**: `tencentcloud_cam_group_membership`
* **New Resource**: `tencentcloud_cam_saml_provider`
* **New Resource**: `tencentcloud_reserved_instance`

ENHANCEMENTS:

* Resource: `tencentcloud_gaap_http_domain` support import
* Resource: `tencentcloud_gaap_layer7_listener` support import

BUG FIXES:

* Resource: `tencentcloud_gaap_http_domain` fix sometimes can't enable realserver auth

## 1.20.1 (October 08, 2019)

ENHANCEMENTS:

* Data Source: `tencentcloud_availability_zones` refactor logic with api3.0 .
* Data Source: `tencentcloud_as_scaling_groups` add optional argument `tags` and attribute `tags`
  for `scaling_group_list`.
* Resource: `tencentcloud_eip` add optional argument `type`, `anycast_zone`, `internet_service_provider`, etc.
* Resource: `tencentcloud_as_scaling_group` add optional argument `tags`.

BUG FIXES:

* Data Source: `tencentcloud_gaap_http_domains` set response `certificate_id`, `client_certificate_id`
  , `realserver_auth`, `basic_auth` and `gaap_auth` default value when they are nil.
* Resource: `tencentcloud_gaap_http_domain` set response `certificate_id`, `client_certificate_id`, `realserver_auth`
  , `basic_auth` and `gaap_auth` default value when they are nil.

## 1.20.0 (September 24, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_eips`
* **New Data Source**: `tencentcloud_instances`
* **New Data Source**: `tencentcloud_key_pairs`
* **New Data Source**: `tencentcloud_placement_groups`
* **New Resource**: `tencentcloud_placement_group`

ENHANCEMENTS:

* Data Source: `tencentcloud_redis_instances` add optional argument `tags`.
* Data Source: `tencentcloud_mongodb_instances` add optional argument `tags`.
* Data Source: `tencentcloud_instance_types` add optional argument `availability_zone` and `gpu_core_count`.
* Data Source: `tencentcloud_gaap_http_rules` add optional argument `forward_host` and attributes `forward_host`
  in `rules`.
* Resource: `tencentcloud_redis_instance` add optional argument `tags`.
* Resource: `tencentcloud_mongodb_instance` add optional argument `tags`.
* Resource: `tencentcloud_mongodb_sharding_instance` add optional argument `tags`.
* Resource: `tencentcloud_instance` add optional argument `placement_group_id`.
* Resource: `tencentcloud_eip` refactor logic with api3.0 .
* Resource: `tencentcloud_eip_association` refactor logic with api3.0 .
* Resource: `tencentcloud_key_pair` refactor logic with api3.0 .
* Resource: `tencentcloud_gaap_http_rule` add optional argument `forward_host`.

BUG FIXES:

* Resource: `tencentcloud_mysql_instance`: miss argument `availability_zone` causes the instance to be recreated.

DEPRECATED:

* Data Source: `tencentcloud_eip` replaced by `tencentcloud_eips`.

## 1.19.0 (September 19, 2019)

FEATURES:

* **New Resource**: `tencentcloud_security_group_lite_rule`.

ENHANCEMENTS:

* Data Source: `tencentcloud_security_groups`: add optional argument `tags`.
* Data Source: `tencentcloud_security_groups`: add optional argument `result_output_file` and new attributes `ingress`
  , `egress` for list `security_groups`.
* Resource: `tencentcloud_security_group`: add optional argument `tags`.
* Resource: `tencentcloud_as_scaling_config`: internet charge type support `BANDWIDTH_PREPAID`
  , `TRAFFIC_POSTPAID_BY_HOUR` and `BANDWIDTH_PACKAGE`.

BUG FIXES:

* Resource: `tencentcloud_clb_listener_rule`: fix unclear description and errors in example.
* Resource: `tencentcloud_instance`: fix hostname is not work.

## 1.18.1 (September 17, 2019)

FEATURES:

* **Update Data Source**: `tencentcloud_vpc_instances` add optional argument `tags`
* **Update Data Source**: `tencentcloud_vpc_subnets` add optional argument `tags`
* **Update Data Source**: `tencentcloud_route_tables` add optional argument `tags`
* **Update Resource**: `tencentcloud_vpc` add optional argument `tags`
* **Update Resource**: `tencentcloud_subnet` add optional argument `tags`
* **Update Resource**: `tencentcloud_route_table` add optional argument `tags`

ENHANCEMENTS:

* Data Source:`tencentcloud_kubernetes_clusters`  support pull out authentication information for cluster access too.
* Resource:`tencentcloud_kubernetes_cluster`  support pull out authentication information for cluster access.

BUG FIXES:

* Resource: `tencentcloud_mysql_instance`: when the mysql is abnormal state, read the basic information report error

DEPRECATED:

* Data Source: `tencentcloud_kubernetes_clusters`:`container_runtime` is no longer supported.

## 1.18.0 (September 10, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_ssl_certificates`
* **New Data Source**: `tencentcloud_dnats`
* **New Data Source**: `tencentcloud_nat_gateways`
* **New Resource**: `tencentcloud_ssl_certificate`
* **Update Resource**: `tencentcloud_clb_redirection` add optional argument `is_auto_rewrite`
* **Update Resource**: `tencentcloud_nat_gateway` , add more configurable items.
* **Update Resource**: `tencentcloud_nat` , add more configurable items.

DEPRECATED:

* Data Source: `tencentcloud_nats` replaced by `tencentcloud_nat_gateways`.

## 1.17.0 (September 04, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_gaap_proxies`
* **New Data Source**: `tencentcloud_gaap_realservers`
* **New Data Source**: `tencentcloud_gaap_layer4_listeners`
* **New Data Source**: `tencentcloud_gaap_layer7_listeners`
* **New Data Source**: `tencentcloud_gaap_http_domains`
* **New Data Source**: `tencentcloud_gaap_http_rules`
* **New Data Source**: `tencentcloud_gaap_security_policies`
* **New Data Source**: `tencentcloud_gaap_security_rules`
* **New Data Source**: `tencentcloud_gaap_certificates`
* **New Resource**: `tencentcloud_gaap_proxy`
* **New Resource**: `tencentcloud_gaap_realserver`
* **New Resource**: `tencentcloud_gaap_layer4_listener`
* **New Resource**: `tencentcloud_gaap_layer7_listener`
* **New Resource**: `tencentcloud_gaap_http_domain`
* **New Resource**: `tencentcloud_gaap_http_rule`
* **New Resource**: `tencentcloud_gaap_certificate`
* **New Resource**: `tencentcloud_gaap_security_policy`
* **New Resource**: `tencentcloud_gaap_security_rule`

## 1.16.3 (August 30, 2019)

BUG FIXIES:

* Resource: `tencentcloud_kubernetes_cluster`: cgi error retry.
* Resource: `tencentcloud_kubernetes_scale_worker`: cgi error retry.

## 1.16.2 (August 28, 2019)

BUG FIXIES:

* Resource: `tencentcloud_instance`: fixed cvm data disks missing computed.
* Resource: `tencentcloud_mysql_backup_policy`: `backup_model` remove logical backup support.
* Resource: `tencentcloud_mysql_instance`: `tags` adapt to the new official api.

## 1.16.1 (August 27, 2019)

ENHANCEMENTS:

* `tencentcloud_instance`: refactor logic with api3.0 .

## 1.16.0 (August 20, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_kubernetes_clusters`
* **New Resource**: `tencentcloud_kubernetes_scale_worker`
* **New Resource**: `tencentcloud_kubernetes_cluster`

DEPRECATED:

* Data Source: `tencentcloud_container_clusters` replaced by `tencentcloud_kubernetes_clusters`.
* Data Source: `tencentcloud_container_cluster_instances` replaced by `tencentcloud_kubernetes_clusters`.
* Resource: `tencentcloud_container_cluster` replaced by `tencentcloud_kubernetes_cluster`.
* Resource: `tencentcloud_container_cluster_instance` replaced by `tencentcloud_kubernetes_scale_worker`.

## 1.15.2 (August 14, 2019)

ENHANCEMENTS:

* `tencentcloud_as_scaling_group`: fixed issue that binding scaling group to load balancer does not work.
* `tencentcloud_clb_attachements`: rename `rewrite_source_rule_id` with `source_rule_id` and
  rename `rewrite_target_rule_id` with `target_rule_id`.

## 1.15.1 (August 13, 2019)

ENHANCEMENTS:

* `tencentcloud_instance`: changed `image_id` property to
  ForceNew ([#78](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/78))
* `tencentcloud_instance`: improved with
  retry ([#82](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/82))
* `tencentcloud_cbs_storages`: improved with
  retry ([#82](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/82))
* `tencentcloud_clb_instance`: bug fixed and improved with
  retry ([#37](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/37))

## 1.15.0 (August 07, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_clb_instances`
* **New Data Source**: `tencentcloud_clb_listeners`
* **New Data Source**: `tencentcloud_clb_listener_rules`
* **New Data Source**: `tencentcloud_clb_attachments`
* **New Data Source**: `tencentcloud_clb_redirections`
* **New Resource**: `tencentcloud_clb_instance`
* **New Resource**: `tencentcloud_clb_listener`
* **New Resource**: `tencentcloud_clb_listener_rule`
* **New Resource**: `tencentcloud_clb_attachment`
* **New Resource**: `tencentcloud_clb_redirection`

DEPRECATED:

* Resource: `tencentcloud_lb` replaced by `tencentcloud_clb_instance`.
* Resource: `tencentcloud_alb_server_attachment` replaced by `tencentcloud_clb_attachment`.

## 1.14.1 (August 05, 2019)

BUG FIXIES:

* resource/tencentcloud_security_group_rule: fixed security group rule id is not compatible with previous version.

## 1.14.0 (July 30, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_security_groups`
* **New Data Source**: `tencentcloud_mongodb_instances`
* **New Data Source**: `tencentcloud_mongodb_zone_config`
* **New Resource**: `tencentcloud_mongodb_instance`
* **New Resource**: `tencentcloud_mongodb_sharding_instance`
* **Update Resource**: `tencentcloud_security_group_rule` add optional argument `description`

DEPRECATED:

* Data Source: `tencnetcloud_security_group` replaced by `tencentcloud_security_groups`

ENHANCEMENTS:

* Refactoring security_group logic with api3.0

## 1.13.0 (July 23, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_dc_gateway_instances`
* **New Data Source**: `tencentcloud_dc_gateway_ccn_routes`
* **New Resource**: `tencentcloud_dc_gateway`
* **New Resource**: `tencentcloud_dc_gateway_ccn_route`

## 1.12.0 (July 16, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_dc_instances`
* **New Data Source**: `tencentcloud_dcx_instances`
* **New Resource**: `tencentcloud_dcx`
* **UPDATE Resource**:`tencentcloud_mysql_instance` and `tencentcloud_mysql_readonly_instance` completely delete
  instance.

BUG FIXIES:

* resource/tencentcloud_instance: fixed issue when data disks set as delete_with_instance not works.
* resource/tencentcloud_instance: if managed public_ip manually, please don't
  define `allocate_public_ip` ([#62](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/62)).
* resource/tencentcloud_eip_association: fixed issue when instances were manually
  deleted ([#60](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/60)).
* resource/tencentcloud_mysql_readonly_instance:remove an unsupported property `gtid`

## 1.11.0 (July 02, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_ccn_instances`
* **New Data Source**: `tencentcloud_ccn_bandwidth_limits`
* **New Resource**: `tencentcloud_ccn`
* **New Resource**: `tencentcloud_ccn_attachment`
* **New Resource**: `tencentcloud_ccn_bandwidth_limit`

## 1.10.0 (June 27, 2019)

ENHANCEMENTS:

* Refactoring vpc logic with api3.0
* Refactoring cbs logic with api3.0

FEATURES:

* **New Data Source**: `tencentcloud_vpc_instances`
* **New Data Source**: `tencentcloud_vpc_subnets`
* **New Data Source**: `tencentcloud_vpc_route_tables`
* **New Data Source**: `tencentcloud_cbs_storages`
* **New Data Source**: `tencentcloud_cbs_snapshots`
* **New Resource**: `tencentcloud_route_table_entry`
* **New Resource**: `tencentcloud_cbs_snapshot_policy`
* **Update Resource**: `tencentcloud_vpc` , add more configurable items.
* **Update Resource**: `tencentcloud_subnet` , add more configurable items.
* **Update Resource**: `tencentcloud_route_table`, add more configurable items.
* **Update Resource**: `tencentcloud_cbs_storage`, add more configurable items.
* **Update Resource**: `tencentcloud_instance`: add optional argument `tags`.
* **Update Resource**: `tencentcloud_security_group_rule`: add optional argument `source_sgid`.

DEPRECATED:

* Data Source: `tencentcloud_vpc` replaced by `tencentcloud_vpc_instances`.
* Data Source: `tencentcloud_subnet` replaced by  `tencentcloud_vpc_subnets`.
* Data Source: `tencentcloud_route_table` replaced by `tencentcloud_vpc_route_tables`.
* Resource: `tencentcloud_route_entry` replaced by `tencentcloud_route_table_entry`.

## 1.9.1 (June 24, 2019)

BUG FIXIES:

* data/tencentcloud_instance: fixed vpc ip is in use error when re-creating with private
  ip ([#46](https://github.com/tencentcloudstack/terraform-provider-tencentcloud/issues/46)).

## 1.9.0 (June 18, 2019)

ENHANCEMENTS:

* update to `v0.12.1` Terraform SDK version

BUG FIXIES:

* data/tencentcloud_security_group: `project_id` remote API return sometime is string type.
* resource/tencentcloud_security_group: just like `data/tencentcloud_security_group`

## 1.8.0 (June 11, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_as_scaling_configs`
* **New Data Source**: `tencentcloud_as_scaling_groups`
* **New Data Source**: `tencentcloud_as_scaling_policies`
* **New Resource**: `tencentcloud_as_scaling_config`
* **New Resource**: `tencentcloud_as_scaling_group`
* **New Resource**: `tencentcloud_as_attachment`
* **New Resource**: `tencentcloud_as_scaling_policy`
* **New Resource**: `tencentcloud_as_schedule`
* **New Resource**: `tencentcloud_as_lifecycle_hook`
* **New Resource**: `tencentcloud_as_notification`

## 1.7.0 (May 23, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_redis_zone_config`
* **New Data Source**: `tencentcloud_redis_instances`
* **New Resource**: `tencentcloud_redis_instance`
* **New Resource**: `tencentcloud_redis_backup_config`

ENHANCEMENTS:

* resource/tencentcloud_instance: Add `hostname`, `project_id`, `delete_with_instance` argument.
* Update tencentcloud-sdk-go to better support redis api.

## 1.6.0 (May 15, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_cos_buckets`
* **New Data Source**: `tencentcloud_cos_bucket_object`
* **New Resource**: `tencentcloud_cos_bucket`
* **New Resource**: `tencentcloud_cos_bucket_object`

ENHANCEMENTS:

* Add the framework of auto generating terraform docs

## 1.5.0 (April 26, 2019)

FEATURES:

* **New Data Source**: `tencentcloud_mysql_backup_list`
* **New Data Source**: `tencentcloud_mysql_zone_config`
* **New Data Source**: `tencentcloud_mysql_parameter_list`
* **New Data Source**: `tencentcloud_mysql_instance`
* **New Resource**: `tencentcloud_mysql_backup_policy`
* **New Resource**: `tencentcloud_mysql_account`
* **New Resource**: `tencentcloud_mysql_account_privilege`
* **New Resource**: `tencentcloud_mysql_instance`
* **New Resource**: `tencentcloud_mysql_readonly_instance`

ENHANCEMENTS:

* resource/tencentcloud_subnet: `route_table_id` now is an optional argument

## 1.4.0 (April 12, 2019)

ENHANCEMENTS:

* data/tencentcloud_image: add `image_name` attribute to this data source.
* resource/tencentcloud_instance: data disk count limit now is upgrade from 1 to 10, as API has supported more disks.
* resource/tencentcloud_instance: PREPAID instance now can be deleted, but still have some limit in API.

BUG FIXIES:

* resource/tencentcloud_instance: `allocate_public_ip` doesn't work properly when it is set to false.

## 1.3.0 (March 12, 2019)

FEATURES:

* **New
  Resource**: `tencentcloud_lb` ([#3](https://github.com/terraform-providers/terraform-provider-scaffolding/issues/3))

ENHANCEMENTS:

* resource/tencentcloud_instance: Add `user_data_raw`
  argument ([#4](https://github.com/terraform-providers/terraform-provider-scaffolding/issues/4))

## 1.2.2 (September 28, 2018)

BUG FIXES:

* resource/tencentcloud_cbs_storage: make name to be
  required ([#25](https://github.com/tencentyun/terraform-provider-tencentcloud/issues/25))
* resource/tencentcloud_instance: support user data and private ip

## 1.2.0 (April 3, 2018)

FEATURES:

* **New Resource**: `tencentcloud_container_cluster`
* **New Resource**: `tencentcloud_container_cluster_instance`
* **New Data Source**: `tencentcloud_container_clusters`
* **New Data Source**: `tencentcloud_container_cluster_instances`

## 1.1.0 (March 9, 2018)

FEATURES:

* **New Resource**: `tencentcloud_eip`
* **New Resource**: `tencentcloud_eip_association`
* **New Data Source**: `tencentcloud_eip`
* **New Resource**: `tencentcloud_nat_gateway`
* **New Resource**: `tencentcloud_dnat`
* **New Data Source**: `tencentcloud_nats`
* **New Resource**: `tencentcloud_cbs_snapshot`
* **New Resource**: `tencentcloud_alb_server_attachment`

## 1.0.0 (January 19, 2018)

FEATURES:

### CVM

RESOURCES:

* instance create
* instance read
* instance update
    * reset instance
    * reset password
    * update instance name
    * update security groups
* instance delete
* key pair create
* key pair read
* key pair delete

DATA SOURCES:

* image read
* instance\_type read
* zone read

### VPC

RESOURCES:

* vpc create
* vpc read
* vpc update (update name)
* vpc delete
* subnet create
* subnet read
* subnet update (update name)
* subnet delete
* security group create
* security group read
* security group update (update name, description)
* security group delete
* security group rule create
* security group rule read
* security group rule delete
* route table create
* route table read
* route table update (update name)
* route table delete
* route entry create
* route entry read
* route entry delete

DATA SOURCES:

* vpc read
* subnet read
* security group read
* route table read

### CBS

RESOURCES:

* storage create
* storage read
* storage update (update name)
* storage attach
* storage detach
