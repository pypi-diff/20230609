# Comparing `tmp/aries_cloudcontroller-0.8.0rc9.tar.gz` & `tmp/aries_cloudcontroller-0.8.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aries_cloudcontroller-0.8.0rc9.tar", last modified: Tue May 23 13:03:03 2023, max compression
+gzip compressed data, was "aries_cloudcontroller-0.8.1rc4.tar", last modified: Fri Jun  9 08:52:14 2023, max compression
```

## Comparing `aries_cloudcontroller-0.8.0rc9.tar` & `aries_cloudcontroller-0.8.1rc4.tar`

### file list

```diff
@@ -1,326 +1,333 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.596993 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/acapy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.600993 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/action_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/basicmessage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/did_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/discover_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/discover_features_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/endorse_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/introduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/issue_credential_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/issue_credential_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/jsonld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/ledger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/mediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/multitenancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/out_of_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/present_proof_v1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/present_proof_v2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/trustping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/
--rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/action_menu_fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status_readiness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/aml_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data1_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data_jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attachment_def.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attribute_mime_types_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/claim_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/clear_pending_revocations_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/conn_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_invitation.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_metadata_set_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_static_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_static_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value_primary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value_revocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_info_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_indy_records_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_record_details_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_record_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_revoked_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definitions_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_status_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_create_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_endpoint_with_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/didx_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_proof_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/disclose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/disclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/endorser_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/endpoints_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_did_endpoint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_did_verkey_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_nym_role_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_attr_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_precis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_ge_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_ge_proof_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_key_correctness_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_non_revocation_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_primary_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/input_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/issuer_cred_rev_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/issuer_rev_reg_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query_filter_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query_paginate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ld_proof_vc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ledger_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ledger_config_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/linked_data_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_grant.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_id_match_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_form_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/model_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/oob_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/perform_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ping_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ping_request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/protocol_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/publish_revocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/query_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/raw_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/receive_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/remove_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/resolution_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_issued_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_regs_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/revoke_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/route_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_get_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_input_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_send_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schemas_created_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/send_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/service_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/sign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/signature_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/signed_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/submission_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_accept.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/tails_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/transaction_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/transaction_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/update_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_exchange_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter_indy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_request_free.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_store_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_ex_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_request_by_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/vc_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/vc_record_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/w3_c_credentials_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/wallet_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/write_ledger_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/uplink_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/util/pydantic_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.596993 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-23 13:03:03.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-05-23 13:03:03.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:03:03.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:03:03.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 13:03:03.000000 aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:03:03.620993 aries_cloudcontroller-0.8.0rc9/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/tests/model/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-23 13:02:53.000000 aries_cloudcontroller-0.8.0rc9/tests/test_acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.658443 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.662443 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/action_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/basicmessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/did_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/discover_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/discover_features_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/endorse_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/introduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/issue_credential_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/issue_credential_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/jsonld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/ledger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/mediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/multitenancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/out_of_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/present_proof_v1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/present_proof_v2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/trustping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/
+-rw-r--r--   0 runner    (1001) docker     (123)    29725 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/action_menu_fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/aml_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data1_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data_jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data_jws_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attachment_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attribute_mime_types_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/claim_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/clear_pending_revocations_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/conn_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_metadata_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_static_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_static_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_def_value_primary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_def_value_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_info_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_rev_indy_records_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_rev_record_details_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_rev_record_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_revoked_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definitions_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_status_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_endpoint_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/didx_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_proof_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/disclose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/disclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/endorser_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/endpoints_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_did_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_did_verkey_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_nym_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_attr_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_precis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_ge_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_ge_proof_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_key_correctness_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_non_revocation_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_primary_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_request_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_entry_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/input_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/issuer_cred_rev_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/issuer_rev_reg_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query_filter_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ld_proof_vc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ld_proof_vc_detail_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ledger_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ledger_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/linked_data_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_id_match_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_form_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/model_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/oob_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/perform_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ping_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ping_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/protocol_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/publish_revocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/query_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/raw_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/receive_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/remove_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/resolution_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_issued_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_regs_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/revoke_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/route_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_input_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schemas_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schemas_input_descriptor_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/send_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/service_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/sign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/signature_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/signed_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/submission_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_accept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/tails_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_publish_revocations_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/update_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_exchange_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_filter_indy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_request_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_discovery_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_issue_cred_schema_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_ex_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_proposal_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_request_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/vc_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/vc_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/w3_c_credentials_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/wallet_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/write_ledger_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/uplink_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/util/create_client_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/util/pydantic_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.658443 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-09 08:52:14.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-09 08:52:14.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:52:14.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-09 08:52:14.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 08:52:14.000000 aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/compare_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:14.686443 aries_cloudcontroller-0.8.1rc4/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/test_credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/test_presentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/test_v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/model/test_v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-09 08:52:05.000000 aries_cloudcontroller-0.8.1rc4/tests/test_acapy_client.py
```

### Comparing `aries_cloudcontroller-0.8.0rc9/LICENSE` & `aries_cloudcontroller-0.8.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/PKG-INFO` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aries_cloudcontroller
-Version: 0.8.0rc9
+Name: aries-cloudcontroller
+Version: 0.8.1rc4
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -55,21 +55,22 @@
 
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
+| 0.8.1                          | 0.8.1                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.0)
+- Supports latest ACA-Py version (0.8.1)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.0rc9 Summary: A
+Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.1rc4 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
 
@@ -17,43 +17,44 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | ## Features Aries Cloud
-Controller Python is a fully featured client for interacting with ACA-Py. -
-Fully Typed wrapper around Aries Cloud Agent Python - Supports latest ACA-Py
-version (0.8.0) - Client is auto generated based on OpenAPI definitions,
-allowing us to keep up to date with new releases. - Supports multi-tenant APIs
-and authentication - Async API ## Usage Aries Cloud Controller Python is
-published to PyPi and can be installed using pip: ```sh pip install aries-
-cloudcontroller ``` ### Creating a client ```python from aries_cloudcontroller
-import AcaPyClient client = AcaPyClient( base_url="http://localhost:8000",
-api_key="myApiKey" ) ``` **Admin insecure mode** If you are running ACA-Py with
-the admin insecure flag and don't have the API key, you must set the
-`admin_insecure` property: ```python client = AcaPyClient( base_url="http://
-localhost:8000", # Explicitly mark that no api key is used admin_insecure=True
-) ``` **Multitenancy** To provision the agent in the context of specific tenant
-of the agent, the `tenant_jwt` property must be set: ```python client =
-AcaPyClient( base_url="http://localhost:8000", tenant_jwt="eyXXX" ) ``` ###
-Interacting with the client Once you have the client set up, you're ready to
-interact with it. Because the API is fully typed, the best way to know what is
-available is by looking at the ACA-Py swagger UI, and the available properties
-on the client. For example to create and receive an invitation the following
-methods can be called: ```python invitation = await
-client.connection.create_invitation( body=CreateInvitationRequest
-(my_label="Cloud Controller") ) connection = await
-client.connection.receive_invitation(body=result.invitation) ``` ## Available
-APIs Currently the following top-level APIs are available in the client. Each
-api maps to the topics as used by the ACA-Py swagger UI. - `action_menu` -
-`basicmessage` - `connection` - `credential_definition` - `credentials` -
-`default` - `did_exchange` - `discover_features` - `discover_features_v2_0` -
-`endorse_transaction` - `introduction` - `issue_credential_v1_0` -
-`issue_credential_v2_0` - `jsonld` - `ledger` - `mediation` - `multitenancy` -
-`out_of_band` - `present_proof_v1_0` - `present_proof_v2_0` - `resolver` -
-`revocation` - `schema` - `server` - `trustping` - `wallet` ## Contributing If
-you would like to contribute to the framework, please read [CONTRIBUTING](/
-CONTRIBUTING.md) guidelines. These documents will provide more information to
-get you started! ## License Aries Cloud Controller Python is licensed under the
-[Apache License Version 2.0 (Apache-2.0)](/LICENSE).
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
+Features Aries Cloud Controller Python is a fully featured client for
+interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
+- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
+OpenAPI definitions, allowing us to keep up to date with new releases. -
+Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
+Controller Python is published to PyPi and can be installed using pip: ```sh
+pip install aries-cloudcontroller ``` ### Creating a client ```python from
+aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
+/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
+running ACA-Py with the admin insecure flag and don't have the API key, you
+must set the `admin_insecure` property: ```python client = AcaPyClient
+( base_url="http://localhost:8000", # Explicitly mark that no api key is used
+admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
+context of specific tenant of the agent, the `tenant_jwt` property must be set:
+```python client = AcaPyClient( base_url="http://localhost:8000",
+tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
+client set up, you're ready to interact with it. Because the API is fully
+typed, the best way to know what is available is by looking at the ACA-Py
+swagger UI, and the available properties on the client. For example to create
+and receive an invitation the following methods can be called: ```python
+invitation = await client.connection.create_invitation
+( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
+await client.connection.receive_invitation(body=result.invitation) ``` ##
+Available APIs Currently the following top-level APIs are available in the
+client. Each api maps to the topics as used by the ACA-Py swagger UI. -
+`action_menu` - `basicmessage` - `connection` - `credential_definition` -
+`credentials` - `default` - `did_exchange` - `discover_features` -
+`discover_features_v2_0` - `endorse_transaction` - `introduction` -
+`issue_credential_v1_0` - `issue_credential_v2_0` - `jsonld` - `ledger` -
+`mediation` - `multitenancy` - `out_of_band` - `present_proof_v1_0` -
+`present_proof_v2_0` - `resolver` - `revocation` - `schema` - `server` -
+`trustping` - `wallet` ## Contributing If you would like to contribute to the
+framework, please read [CONTRIBUTING](/CONTRIBUTING.md) guidelines. These
+documents will provide more information to get you started! ## License Aries
+Cloud Controller Python is licensed under the [Apache License Version 2.0
+(Apache-2.0)](/LICENSE).
```

### Comparing `aries_cloudcontroller-0.8.0rc9/README.md` & `aries_cloudcontroller-0.8.1rc4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,22 @@
 
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
+| 0.8.1                          | 0.8.1                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.0)
+- Supports latest ACA-Py version (0.8.1)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -10,43 +10,44 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | ## Features Aries Cloud
-Controller Python is a fully featured client for interacting with ACA-Py. -
-Fully Typed wrapper around Aries Cloud Agent Python - Supports latest ACA-Py
-version (0.8.0) - Client is auto generated based on OpenAPI definitions,
-allowing us to keep up to date with new releases. - Supports multi-tenant APIs
-and authentication - Async API ## Usage Aries Cloud Controller Python is
-published to PyPi and can be installed using pip: ```sh pip install aries-
-cloudcontroller ``` ### Creating a client ```python from aries_cloudcontroller
-import AcaPyClient client = AcaPyClient( base_url="http://localhost:8000",
-api_key="myApiKey" ) ``` **Admin insecure mode** If you are running ACA-Py with
-the admin insecure flag and don't have the API key, you must set the
-`admin_insecure` property: ```python client = AcaPyClient( base_url="http://
-localhost:8000", # Explicitly mark that no api key is used admin_insecure=True
-) ``` **Multitenancy** To provision the agent in the context of specific tenant
-of the agent, the `tenant_jwt` property must be set: ```python client =
-AcaPyClient( base_url="http://localhost:8000", tenant_jwt="eyXXX" ) ``` ###
-Interacting with the client Once you have the client set up, you're ready to
-interact with it. Because the API is fully typed, the best way to know what is
-available is by looking at the ACA-Py swagger UI, and the available properties
-on the client. For example to create and receive an invitation the following
-methods can be called: ```python invitation = await
-client.connection.create_invitation( body=CreateInvitationRequest
-(my_label="Cloud Controller") ) connection = await
-client.connection.receive_invitation(body=result.invitation) ``` ## Available
-APIs Currently the following top-level APIs are available in the client. Each
-api maps to the topics as used by the ACA-Py swagger UI. - `action_menu` -
-`basicmessage` - `connection` - `credential_definition` - `credentials` -
-`default` - `did_exchange` - `discover_features` - `discover_features_v2_0` -
-`endorse_transaction` - `introduction` - `issue_credential_v1_0` -
-`issue_credential_v2_0` - `jsonld` - `ledger` - `mediation` - `multitenancy` -
-`out_of_band` - `present_proof_v1_0` - `present_proof_v2_0` - `resolver` -
-`revocation` - `schema` - `server` - `trustping` - `wallet` ## Contributing If
-you would like to contribute to the framework, please read [CONTRIBUTING](/
-CONTRIBUTING.md) guidelines. These documents will provide more information to
-get you started! ## License Aries Cloud Controller Python is licensed under the
-[Apache License Version 2.0 (Apache-2.0)](/LICENSE).
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
+Features Aries Cloud Controller Python is a fully featured client for
+interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
+- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
+OpenAPI definitions, allowing us to keep up to date with new releases. -
+Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
+Controller Python is published to PyPi and can be installed using pip: ```sh
+pip install aries-cloudcontroller ``` ### Creating a client ```python from
+aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
+/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
+running ACA-Py with the admin insecure flag and don't have the API key, you
+must set the `admin_insecure` property: ```python client = AcaPyClient
+( base_url="http://localhost:8000", # Explicitly mark that no api key is used
+admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
+context of specific tenant of the agent, the `tenant_jwt` property must be set:
+```python client = AcaPyClient( base_url="http://localhost:8000",
+tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
+client set up, you're ready to interact with it. Because the API is fully
+typed, the best way to know what is available is by looking at the ACA-Py
+swagger UI, and the available properties on the client. For example to create
+and receive an invitation the following methods can be called: ```python
+invitation = await client.connection.create_invitation
+( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
+await client.connection.receive_invitation(body=result.invitation) ``` ##
+Available APIs Currently the following top-level APIs are available in the
+client. Each api maps to the topics as used by the ACA-Py swagger UI. -
+`action_menu` - `basicmessage` - `connection` - `credential_definition` -
+`credentials` - `default` - `did_exchange` - `discover_features` -
+`discover_features_v2_0` - `endorse_transaction` - `introduction` -
+`issue_credential_v1_0` - `issue_credential_v2_0` - `jsonld` - `ledger` -
+`mediation` - `multitenancy` - `out_of_band` - `present_proof_v1_0` -
+`present_proof_v2_0` - `resolver` - `revocation` - `schema` - `server` -
+`trustping` - `wallet` ## Contributing If you would like to contribute to the
+framework, please read [CONTRIBUTING](/CONTRIBUTING.md) guidelines. These
+documents will provide more information to get you started! ## License Aries
+Cloud Controller Python is licensed under the [Apache License Version 2.0
+(Apache-2.0)](/LICENSE).
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/__init__.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/__init__.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/action_menu.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/action_menu.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/basicmessage.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/basicmessage.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/connection.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     CreateInvitationRequest,
 )
 from aries_cloudcontroller.model.endpoints_result import EndpointsResult
 from aries_cloudcontroller.model.invitation_result import InvitationResult
 from aries_cloudcontroller.model.receive_invitation_request import (
     ReceiveInvitationRequest,
 )
-from aries_cloudcontroller.uplink_util import bool_query
 
 
 class ConnectionApi(Consumer):
     async def accept_invitation(
         self,
         *,
         conn_id: str,
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/credential_definition.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/credential_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.credential_definition_get_result import (
     CredentialDefinitionGetResult,
 )
 from aries_cloudcontroller.model.credential_definition_send_request import (
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/credentials.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/credentials.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/did_exchange.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/did_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.conn_record import ConnRecord
 from aries_cloudcontroller.model.didx_request import DIDXRequest
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/discover_features.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/discover_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.v10_discovery_exchange_list_result import (
     V10DiscoveryExchangeListResult,
 )
 from aries_cloudcontroller.model.v10_discovery_record import V10DiscoveryRecord
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/discover_features_v2_0.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/discover_features_v2_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.v20_discovery_exchange_list_result import (
     V20DiscoveryExchangeListResult,
 )
 from aries_cloudcontroller.model.v20_discovery_exchange_result import (
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/endorse_transaction.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/endorse_transaction.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.date import Date
 from aries_cloudcontroller.model.endorser_info import EndorserInfo
 from aries_cloudcontroller.model.transaction_jobs import TransactionJobs
 from aries_cloudcontroller.model.transaction_list import TransactionList
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/introduction.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/introduction.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/issue_credential_v1_0.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/issue_credential_v1_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/issue_credential_v2_0.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/issue_credential_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/jsonld.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/jsonld.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.sign_request import SignRequest
 from aries_cloudcontroller.model.sign_response import SignResponse
 from aries_cloudcontroller.model.verify_request import VerifyRequest
 from aries_cloudcontroller.model.verify_response import VerifyResponse
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/ledger.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/ledger.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from aries_cloudcontroller.model.ledger_config_list import LedgerConfigList
 from aries_cloudcontroller.model.taa_accept import TAAAccept
 from aries_cloudcontroller.model.taa_result import TAAResult
 from aries_cloudcontroller.model.txn_or_register_ledger_nym_response import (
     TxnOrRegisterLedgerNymResponse,
 )
 from aries_cloudcontroller.model.write_ledger_request import WriteLedgerRequest
-from aries_cloudcontroller.uplink_util import bool_query
 
 
 class LedgerApi(Consumer):
     async def accept_taa(self, *, body: Optional[TAAAccept] = None) -> Dict[str, Any]:
         """Accept the transaction author agreement"""
         return await self.__accept_taa(
             body=body,
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/mediation.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/mediation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.admin_mediation_deny import AdminMediationDeny
 from aries_cloudcontroller.model.keylist import Keylist
 from aries_cloudcontroller.model.keylist_query import KeylistQuery
 from aries_cloudcontroller.model.keylist_query_filter_request import (
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/multitenancy.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/multitenancy.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/out_of_band.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/out_of_band.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.invitation_create_request import (
     InvitationCreateRequest,
 )
 from aries_cloudcontroller.model.invitation_message import InvitationMessage
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/present_proof_v1_0.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/present_proof_v1_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/present_proof_v2_0.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/present_proof_v2_0.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/resolver.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.resolution_result import ResolutionResult
 
 
 class ResolverApi(Consumer):
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/revocation.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/revocation.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     async def publish_rev_reg_def(
         self,
         *,
         rev_reg_id: str,
         conn_id: Optional[str] = None,
         create_transaction_for_endorser: Optional[bool] = None
-    ) -> TxnOrRevRegResult:
+    ) -> Union[RevRegResult, TxnOrRevRegResult]:
         """Send revocation registry definition to ledger"""
         return await self.__publish_rev_reg_def(
             rev_reg_id=rev_reg_id,
             conn_id=conn_id,
             create_transaction_for_endorser=bool_query(create_transaction_for_endorser),
         )
 
@@ -275,15 +275,15 @@
     @post("/revocation/registry/{rev_reg_id}/definition")
     def __publish_rev_reg_def(
         self,
         *,
         rev_reg_id: str,
         conn_id: Query = None,
         create_transaction_for_endorser: Query = None
-    ) -> TxnOrRevRegResult:
+    ) -> Union[RevRegResult, TxnOrRevRegResult]:
         """Internal uplink method for publish_rev_reg_def"""
 
     @returns.json
     @post("/revocation/registry/{rev_reg_id}/entry")
     def __publish_rev_reg_entry(
         self,
         *,
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/schema.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.schema_get_result import SchemaGetResult
 from aries_cloudcontroller.model.schema_send_request import SchemaSendRequest
 from aries_cloudcontroller.model.schemas_created_result import SchemasCreatedResult
 from aries_cloudcontroller.model.txn_or_schema_send_result import TxnOrSchemaSendResult
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/server.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/server.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/trustping.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/trustping.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     patch,
     put,
     delete,
     returns,
     json,
 )
 
-from typing import Dict, List, Optional, Union  # noqa: F401
+from typing import Any, Dict, List, Optional, Union  # noqa: F401
 
 from aries_cloudcontroller.uplink_util import bool_query
 
 from aries_cloudcontroller.model.ping_request import PingRequest
 from aries_cloudcontroller.model.ping_request_response import PingRequestResponse
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/api/wallet.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/api/wallet.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/client.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from contextlib import AbstractAsyncContextManager
 from typing import Dict
 
 import uplink
-
 from aries_cloudcontroller.api import (
     ActionMenuApi,
     BasicmessageApi,
     ConnectionApi,
     CredentialDefinitionApi,
     CredentialsApi,
     DefaultApi,
@@ -65,18 +64,20 @@
         self,
         base_url: str,
         client: uplink.AiohttpClient,
         *,
         extra_service_params: Dict = {}
     ):
         self.base_url = base_url
+        self.client = client
+
         service_params = {
             **extra_service_params,
-            "base_url": base_url,
-            "client": client,
+            "base_url": self.base_url,
+            "client": self.client,
         }
 
         self.action_menu = ActionMenuApi(**service_params)
         self.basicmessage = BasicmessageApi(**service_params)
         self.connection = ConnectionApi(**service_params)
         self.credential_definition = CredentialDefinitionApi(**service_params)
         self.credentials = CredentialsApi(**service_params)
@@ -98,14 +99,12 @@
         self.resolver = ResolverApi(**service_params)
         self.revocation = RevocationApi(**service_params)
         self.schema = SchemaApi(**service_params)
         self.server = ServerApi(**service_params)
         self.trustping = TrustpingApi(**service_params)
         self.wallet = WalletApi(**service_params)
 
-        self.client = client
-
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.client.close()
 
     async def close(self):
         await self.client.close()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/__init__.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/action_menu_fetch_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/action_menu_fetch_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     ActionMenuFetchResult - a model defined in OpenAPI
         result: Action menu [Optional].
     """
 
     result: Optional[Menu] = None
 
-    def __init__(
-        self,
-        *,
-        result: Optional[Menu] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 ActionMenuFetchResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_config.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/tails_delete_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class AdminConfig(BaseModel):
+class TailsDeleteResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    AdminConfig - a model defined in OpenAPI
-        config: Configuration settings [Optional].
+    TailsDeleteResponse - a model defined in OpenAPI
+        message: The message of this TailsDeleteResponse [Optional].
     """
 
-    config: Optional[Dict[str, Any]] = None
-
-    def __init__(
-        self,
-        *,
-        config: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            config=config,
-            **kwargs,
-        )
+    message: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-AdminConfig.update_forward_refs()
+TailsDeleteResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_mediation_deny.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_mediation_deny.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         mediator_terms: List of mediator rules for recipient [Optional].
         recipient_terms: List of recipient rules for mediation [Optional].
     """
 
     mediator_terms: Optional[List[str]] = None
     recipient_terms: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        mediator_terms: Optional[List[str]] = None,
-        recipient_terms: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mediator_terms=mediator_terms,
-            recipient_terms=recipient_terms,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AdminMediationDeny.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_modules.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_modules.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     AdminModules - a model defined in OpenAPI
         result: List of admin modules [Optional].
     """
 
     result: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        result: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AdminModules.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,29 +23,12 @@
     """
 
     conductor: Optional[Dict[str, Any]] = None
     label: Optional[str] = None
     timing: Optional[Dict[str, Any]] = None
     version: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        conductor: Optional[Dict[str, Any]] = None,
-        label: Optional[str] = None,
-        timing: Optional[Dict[str, Any]] = None,
-        version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            conductor=conductor,
-            label=label,
-            timing=timing,
-            version=version,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AdminStatus.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status_liveliness.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status_liveliness.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     AdminStatusLiveliness - a model defined in OpenAPI
         alive: Liveliness status [Optional].
     """
 
     alive: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        alive: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            alive=alive,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AdminStatusLiveliness.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/admin_status_readiness.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_status_readiness.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     AdminStatusReadiness - a model defined in OpenAPI
         ready: Readiness status [Optional].
     """
 
     ready: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        ready: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            ready=ready,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AdminStatusReadiness.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/aml_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/aml_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         version: The version of this AMLRecord [Optional].
     """
 
     aml: Optional[Dict[str, str]] = None
     aml_context: Optional[str] = Field(None, alias="amlContext")
     version: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        aml: Optional[Dict[str, str]] = None,
-        aml_context: Optional[str] = None,
-        version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            aml=aml,
-            aml_context=aml_context,
-            version=version,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AMLRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,74 +4,66 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attach_decorator_data import AttachDecoratorData
+from aries_cloudcontroller.model.indy_proof_req_attr_spec import IndyProofReqAttrSpec
+from aries_cloudcontroller.model.indy_proof_req_pred_spec import IndyProofReqPredSpec
+from aries_cloudcontroller.model.indy_proof_request_non_revoked import (
+    IndyProofRequestNonRevoked,
+)
 
 
-class AttachDecorator(BaseModel):
+class IndyProofRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    AttachDecorator - a model defined in OpenAPI
-        data: The data of this AttachDecorator.
-        id: Attachment identifier [Optional].
-        byte_count: Byte count of data included by reference [Optional].
-        description: Human-readable description of content [Optional].
-        filename: File name [Optional].
-        lastmod_time: Hint regarding last modification datetime, in ISO-8601 format [Optional].
-        mime_type: MIME type [Optional].
+    IndyProofRequest - a model defined in OpenAPI
+        requested_attributes: Requested attribute specifications of proof request.
+        requested_predicates: Requested predicate specifications of proof request.
+        name: Proof request name [Optional].
+        non_revoked: The non_revoked of this IndyProofRequest [Optional].
+        nonce: Nonce [Optional].
+        version: Proof request version [Optional].
     """
 
-    data: AttachDecoratorData
-    id: Optional[str] = Field(None, alias="@id")
-    byte_count: Optional[int] = None
-    description: Optional[str] = None
-    filename: Optional[str] = None
-    lastmod_time: Optional[str] = None
-    mime_type: Optional[str] = Field(None, alias="mime-type")
-
-    def __init__(
-        self,
-        *,
-        data: AttachDecoratorData = None,
-        id: Optional[str] = None,
-        byte_count: Optional[int] = None,
-        description: Optional[str] = None,
-        filename: Optional[str] = None,
-        lastmod_time: Optional[str] = None,
-        mime_type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            byte_count=byte_count,
-            data=data,
-            description=description,
-            filename=filename,
-            lastmod_time=lastmod_time,
-            mime_type=mime_type,
-            **kwargs,
-        )
+    requested_attributes: Dict[str, IndyProofReqAttrSpec]
+    requested_predicates: Dict[str, IndyProofReqPredSpec]
+    name: Optional[str] = None
+    non_revoked: Optional[IndyProofRequestNonRevoked] = None
+    nonce: Optional[str] = None
+    version: Optional[str] = None
 
-    @validator("lastmod_time")
-    def lastmod_time_pattern(cls, value):
+    @validator("nonce")
+    def nonce_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        pattern = r"^[1-9][0-9]*$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of lastmod_time does not match regex pattern ('{pattern}')"
+                f"Value of nonce does not match regex pattern ('{pattern}')"
+            )
+        return value
+
+    @validator("version")
+    def version_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[0-9.]+$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of version does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-AttachDecorator.update_forward_refs()
+IndyProofRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,33 +26,14 @@
 
     base64: Optional[str] = None
     json_: Optional[Dict[str, Any]] = Field(None, alias="json")
     jws: Optional[AttachDecoratorDataJWS] = None
     links: Optional[List[str]] = None
     sha256: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        base64: Optional[str] = None,
-        json_: Optional[Dict[str, Any]] = None,
-        jws: Optional[AttachDecoratorDataJWS] = None,
-        links: Optional[List[str]] = None,
-        sha256: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            base64=base64,
-            json_=json_,
-            jws=jws,
-            links=links,
-            sha256=sha256,
-            **kwargs,
-        )
-
     @validator("base64")
     def base64_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[a-zA-Z0-9+\/]*={0,2}$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data1_jws.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data1_jws.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,29 +24,14 @@
         protected: protected JWS header [Optional].
     """
 
     header: AttachDecoratorDataJWSHeader
     signature: str
     protected: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        header: AttachDecoratorDataJWSHeader = None,
-        signature: str = None,
-        protected: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            header=header,
-            protected=protected,
-            signature=signature,
-            **kwargs,
-        )
-
     @validator("protected")
     def protected_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[-_a-zA-Z0-9]*$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data_jws.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator_data_jws.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,31 +29,14 @@
     """
 
     header: Optional[AttachDecoratorDataJWSHeader] = None
     protected: Optional[str] = None
     signature: Optional[str] = None
     signatures: Optional[List[AttachDecoratorData1JWS]] = None
 
-    def __init__(
-        self,
-        *,
-        header: Optional[AttachDecoratorDataJWSHeader] = None,
-        protected: Optional[str] = None,
-        signature: Optional[str] = None,
-        signatures: Optional[List[AttachDecoratorData1JWS]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            header=header,
-            protected=protected,
-            signature=signature,
-            signatures=signatures,
-            **kwargs,
-        )
-
     @validator("protected")
     def protected_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[-_a-zA-Z0-9]*$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attach_decorator_data_jws_header.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_endpoint.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,41 +6,45 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class AttachDecoratorDataJWSHeader(BaseModel):
+class DIDEndpoint(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    AttachDecoratorDataJWSHeader - a model defined in OpenAPI
-        kid: Key identifier, in W3C did:key or DID URL format.
+    DIDEndpoint - a model defined in OpenAPI
+        did: DID of interest.
+        endpoint: Endpoint to set (omit to delete) [Optional].
     """
 
-    kid: str
+    did: str
+    endpoint: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        kid: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            kid=kid,
-            **kwargs,
-        )
-
-    @validator("kid")
-    def kid_pattern(cls, value):
-        pattern = r"^did:(?:key:z[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]+|sov:[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}(;.*)?(\?.*)?#.+)$"
+    @validator("did")
+    def did_pattern(cls, value):
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of kid does not match regex pattern ('{pattern}')")
+            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
+        return value
+
+    @validator("endpoint")
+    def endpoint_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[A-Za-z0-9\.\-\+]+:\/\/([A-Za-z0-9][.A-Za-z0-9-_]+[A-Za-z0-9])+(:[1-9][0-9]*)?(\/[^?&#]+)?$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of endpoint does not match regex pattern ('{pattern}')"
+            )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-AttachDecoratorDataJWSHeader.update_forward_refs()
+DIDEndpoint.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attachment_def.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attachment_def.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         id: Attachment identifier [Optional].
         type: Attachment type [Optional].
     """
 
     id: Optional[str] = None
     type: Optional[Literal["credential-offer", "present-proof"]] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[Literal["credential-offer", "present-proof"]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 AttachmentDef.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/attribute_mime_types_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/vc_record_list.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,36 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.vc_record import VCRecord
 
 
-class AttributeMimeTypesResult(BaseModel):
+class VCRecordList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    AttributeMimeTypesResult - a model defined in OpenAPI
-        results: The results of this AttributeMimeTypesResult [Optional].
+    VCRecordList - a model defined in OpenAPI
+        results: The results of this VCRecordList [Optional].
     """
 
-    results: Optional[Dict[str, str]] = None
-
-    def __init__(
-        self,
-        *,
-        results: Optional[Dict[str, str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
+    results: Optional[List[VCRecord]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-AttributeMimeTypesResult.update_forward_refs()
+VCRecordList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/claim_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/claim_format.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,33 +27,12 @@
     jwt: Optional[Dict[str, Any]] = None
     jwt_vc: Optional[Dict[str, Any]] = None
     jwt_vp: Optional[Dict[str, Any]] = None
     ldp: Optional[Dict[str, Any]] = None
     ldp_vc: Optional[Dict[str, Any]] = None
     ldp_vp: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        jwt: Optional[Dict[str, Any]] = None,
-        jwt_vc: Optional[Dict[str, Any]] = None,
-        jwt_vp: Optional[Dict[str, Any]] = None,
-        ldp: Optional[Dict[str, Any]] = None,
-        ldp_vc: Optional[Dict[str, Any]] = None,
-        ldp_vp: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            jwt=jwt,
-            jwt_vc=jwt_vc,
-            jwt_vp=jwt_vp,
-            ldp=ldp,
-            ldp_vc=ldp_vc,
-            ldp_vp=ldp_vp,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 ClaimFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/clear_pending_revocations_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/clear_pending_revocations_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     ClearPendingRevocationsRequest - a model defined in OpenAPI
         purge: Credential revocation ids by revocation registry id: omit for all, specify null or empty list for all pending per revocation registry [Optional].
     """
 
     purge: Optional[Dict[str, List[str]]] = None
 
-    def __init__(
-        self,
-        *,
-        purge: Optional[Dict[str, List[str]]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            purge=purge,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 ClearPendingRevocationsRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     ConnectionList - a model defined in OpenAPI
         results: List of connection records [Optional].
     """
 
     results: Optional[List[ConnRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[ConnRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 ConnectionList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_metadata.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     ConnectionMetadata - a model defined in OpenAPI
         results: Dictionary of metadata associated with connection. [Optional].
     """
 
     results: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 ConnectionMetadata.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_metadata_set_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/resolution_result.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ConnectionMetadataSetRequest(BaseModel):
+class ResolutionResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ConnectionMetadataSetRequest - a model defined in OpenAPI
-        metadata: Dictionary of metadata to set for connection..
+    ResolutionResult - a model defined in OpenAPI
+        did_document: DID Document.
+        metadata: Resolution metadata.
     """
 
+    did_document: Dict[str, Any]
     metadata: Dict[str, Any]
 
-    def __init__(
-        self,
-        *,
-        metadata: Dict[str, Any] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            metadata=metadata,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
-ConnectionMetadataSetRequest.update_forward_refs()
+ResolutionResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_static_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_static_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,39 +31,14 @@
     my_seed: Optional[str] = None
     their_did: Optional[str] = None
     their_endpoint: Optional[str] = None
     their_label: Optional[str] = None
     their_seed: Optional[str] = None
     their_verkey: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        alias: Optional[str] = None,
-        my_did: Optional[str] = None,
-        my_seed: Optional[str] = None,
-        their_did: Optional[str] = None,
-        their_endpoint: Optional[str] = None,
-        their_label: Optional[str] = None,
-        their_seed: Optional[str] = None,
-        their_verkey: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            alias=alias,
-            my_did=my_did,
-            my_seed=my_seed,
-            their_did=their_did,
-            their_endpoint=their_endpoint,
-            their_label=their_label,
-            their_seed=their_seed,
-            their_verkey=their_verkey,
-            **kwargs,
-        )
-
     @validator("my_did")
     def my_did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/connection_static_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_static_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,35 +28,14 @@
     my_did: str
     my_endpoint: str
     my_verkey: str
     record: ConnRecord
     their_did: str
     their_verkey: str
 
-    def __init__(
-        self,
-        *,
-        my_did: str = None,
-        my_endpoint: str = None,
-        my_verkey: str = None,
-        record: ConnRecord = None,
-        their_did: str = None,
-        their_verkey: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            my_did=my_did,
-            my_endpoint=my_endpoint,
-            my_verkey=my_verkey,
-            record=record,
-            their_did=their_did,
-            their_verkey=their_verkey,
-            **kwargs,
-        )
-
     @validator("my_did")
     def my_did_pattern(cls, value):
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of my_did does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/constraints.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/constraints.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,35 +31,12 @@
     is_holder: Optional[List[DIFHolder]] = None
     limit_disclosure: Optional[str] = None
     status_active: Optional[Literal["required", "allowed", "disallowed"]] = None
     status_revoked: Optional[Literal["required", "allowed", "disallowed"]] = None
     status_suspended: Optional[Literal["required", "allowed", "disallowed"]] = None
     subject_is_issuer: Optional[Literal["required", "preferred"]] = None
 
-    def __init__(
-        self,
-        *,
-        fields: Optional[List[DIFField]] = None,
-        is_holder: Optional[List[DIFHolder]] = None,
-        limit_disclosure: Optional[str] = None,
-        status_active: Optional[Literal["required", "allowed", "disallowed"]] = None,
-        status_revoked: Optional[Literal["required", "allowed", "disallowed"]] = None,
-        status_suspended: Optional[Literal["required", "allowed", "disallowed"]] = None,
-        subject_is_issuer: Optional[Literal["required", "preferred"]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            fields=fields,
-            is_holder=is_holder,
-            limit_disclosure=limit_disclosure,
-            status_active=status_active,
-            status_revoked=status_revoked,
-            status_suspended=status_suspended,
-            subject_is_issuer=subject_is_issuer,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 Constraints.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_invitation_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_invitation_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,35 +27,14 @@
     mediation_id: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     my_label: Optional[str] = None
     recipient_keys: Optional[List[str]] = None
     routing_keys: Optional[List[str]] = None
     service_endpoint: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        mediation_id: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        my_label: Optional[str] = None,
-        recipient_keys: Optional[List[str]] = None,
-        routing_keys: Optional[List[str]] = None,
-        service_endpoint: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mediation_id=mediation_id,
-            metadata=metadata,
-            my_label=my_label,
-            recipient_keys=recipient_keys,
-            routing_keys=routing_keys,
-            service_endpoint=service_endpoint,
-            **kwargs,
-        )
-
     @validator("mediation_id")
     def mediation_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-4[a-fA-F0-9]{3}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,37 +29,14 @@
     wallet_id: str
     created_at: Optional[str] = None
     settings: Optional[Dict[str, Any]] = None
     state: Optional[str] = None
     token: Optional[str] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        key_management_mode: Literal["managed", "unmanaged"] = None,
-        wallet_id: str = None,
-        created_at: Optional[str] = None,
-        settings: Optional[Dict[str, Any]] = None,
-        state: Optional[str] = None,
-        token: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            key_management_mode=key_management_mode,
-            settings=settings,
-            state=state,
-            token=token,
-            updated_at=updated_at,
-            wallet_id=wallet_id,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_token_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/create_wallet_token_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class CreateWalletTokenRequest(BaseModel):
+class CreateWalletTokenResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CreateWalletTokenRequest - a model defined in OpenAPI
-        wallet_key: Master key used for key derivation. Only required for             unamanged wallets. [Optional].
+    CreateWalletTokenResponse - a model defined in OpenAPI
+        token: Authorization token to authenticate wallet requests [Optional].
     """
 
-    wallet_key: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        wallet_key: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            wallet_key=wallet_key,
-            **kwargs,
-        )
+    token: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CreateWalletTokenRequest.update_forward_refs()
+CreateWalletTokenResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/create_wallet_token_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/queries.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,36 +4,30 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.query_item import QueryItem
 
 
-class CreateWalletTokenResponse(BaseModel):
+class Queries(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CreateWalletTokenResponse - a model defined in OpenAPI
-        token: Authorization token to authenticate wallet requests [Optional].
+    Queries - a model defined in OpenAPI
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        queries: The queries of this Queries [Optional].
     """
 
-    token: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        token: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            token=token,
-            **kwargs,
-        )
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    queries: Optional[List[QueryItem]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CreateWalletTokenResponse.update_forward_refs()
+Queries.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_attr_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_attr_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         mime_type: MIME type: omit for (null) default [Optional].
     """
 
     name: str
     value: str
     mime_type: Optional[str] = Field(None, alias="mime-type")
 
-    def __init__(
-        self,
-        *,
-        name: str = None,
-        value: str = None,
-        mime_type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mime_type=mime_type,
-            name=name,
-            value=value,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredAttrSpec.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_send_request_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,42 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.cred_def_value_primary import CredDefValuePrimary
-from aries_cloudcontroller.model.cred_def_value_revocation import CredDefValueRevocation
+from aries_cloudcontroller.model.v20_pres_request_by_format import (
+    V20PresRequestByFormat,
+)
 
 
-class CredDefValue(BaseModel):
+class V20PresSendRequestRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredDefValue - a model defined in OpenAPI
-        primary: Primary value for credential definition [Optional].
-        revocation: Revocation value for credential definition [Optional].
+    V20PresSendRequestRequest - a model defined in OpenAPI
+        connection_id: Connection identifier.
+        presentation_request: The presentation_request of this V20PresSendRequestRequest.
+        auto_verify: Verifier choice to auto-verify proof presentation [Optional].
+        comment: The comment of this V20PresSendRequestRequest [Optional].
+        trace: Whether to trace event (default false) [Optional].
     """
 
-    primary: Optional[CredDefValuePrimary] = None
-    revocation: Optional[CredDefValueRevocation] = None
-
-    def __init__(
-        self,
-        *,
-        primary: Optional[CredDefValuePrimary] = None,
-        revocation: Optional[CredDefValueRevocation] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            primary=primary,
-            revocation=revocation,
-            **kwargs,
-        )
+    connection_id: str
+    presentation_request: V20PresRequestByFormat
+    auto_verify: Optional[bool] = None
+    comment: Optional[str] = None
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredDefValue.update_forward_refs()
+V20PresSendRequestRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value_primary.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/generated.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,99 +4,68 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.generated import Generated
 
 
-class CredDefValuePrimary(BaseModel):
+class Generated(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredDefValuePrimary - a model defined in OpenAPI
-        n: The n of this CredDefValuePrimary [Optional].
-        r: The r of this CredDefValuePrimary [Optional].
-        rctxt: The rctxt of this CredDefValuePrimary [Optional].
-        s: The s of this CredDefValuePrimary [Optional].
-        z: The z of this CredDefValuePrimary [Optional].
+    Generated - a model defined in OpenAPI
+        master_secret: The master_secret of this Generated [Optional].
+        number: The number of this Generated [Optional].
+        remainder: The remainder of this Generated [Optional].
     """
 
-    n: Optional[str] = None
-    r: Optional[Generated] = None
-    rctxt: Optional[str] = None
-    s: Optional[str] = None
-    z: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        n: Optional[str] = None,
-        r: Optional[Generated] = None,
-        rctxt: Optional[str] = None,
-        s: Optional[str] = None,
-        z: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            n=n,
-            r=r,
-            rctxt=rctxt,
-            s=s,
-            z=z,
-            **kwargs,
-        )
+    master_secret: Optional[str] = None
+    number: Optional[str] = None
+    remainder: Optional[str] = None
 
-    @validator("n")
-    def n_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^[0-9]*$"
-        if not re.match(pattern, value):
-            raise ValueError(f"Value of n does not match regex pattern ('{pattern}')")
-        return value
-
-    @validator("rctxt")
-    def rctxt_pattern(cls, value):
+    @validator("master_secret")
+    def master_secret_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of rctxt does not match regex pattern ('{pattern}')"
+                f"Value of master_secret does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("s")
-    def s_pattern(cls, value):
+    @validator("number")
+    def number_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of s does not match regex pattern ('{pattern}')")
+            raise ValueError(
+                f"Value of number does not match regex pattern ('{pattern}')"
+            )
         return value
 
-    @validator("z")
-    def z_pattern(cls, value):
+    @validator("remainder")
+    def remainder_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of z does not match regex pattern ('{pattern}')")
+            raise ValueError(
+                f"Value of remainder does not match regex pattern ('{pattern}')"
+            )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredDefValuePrimary.update_forward_refs()
+Generated.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_def_value_revocation.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_def_value_revocation.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,43 +37,12 @@
     h2: Optional[str] = None
     h_cap: Optional[str] = None
     htilde: Optional[str] = None
     pk: Optional[str] = None
     u: Optional[str] = None
     y: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        g: Optional[str] = None,
-        g_dash: Optional[str] = None,
-        h: Optional[str] = None,
-        h0: Optional[str] = None,
-        h1: Optional[str] = None,
-        h2: Optional[str] = None,
-        h_cap: Optional[str] = None,
-        htilde: Optional[str] = None,
-        pk: Optional[str] = None,
-        u: Optional[str] = None,
-        y: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            g=g,
-            g_dash=g_dash,
-            h=h,
-            h0=h0,
-            h1=h1,
-            h2=h2,
-            h_cap=h_cap,
-            htilde=htilde,
-            pk=pk,
-            u=u,
-            y=y,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredDefValueRevocation.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_info_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_info_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     CredInfoList - a model defined in OpenAPI
         results: The results of this CredInfoList [Optional].
     """
 
     results: Optional[List[IndyCredInfo]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[IndyCredInfo]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredInfoList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_indy_records_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.did import DID
 
 
-class CredRevIndyRecordsResult(BaseModel):
+class DIDResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredRevIndyRecordsResult - a model defined in OpenAPI
-        rev_reg_delta: Indy revocation registry delta [Optional].
+    DIDResult - a model defined in OpenAPI
+        result: The result of this DIDResult [Optional].
     """
 
-    rev_reg_delta: Optional[Dict[str, Any]] = None
-
-    def __init__(
-        self,
-        *,
-        rev_reg_delta: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            rev_reg_delta=rev_reg_delta,
-            **kwargs,
-        )
+    result: Optional[DID] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredRevIndyRecordsResult.update_forward_refs()
+DIDResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_record_details_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_rev_record_details_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     CredRevRecordDetailsResult - a model defined in OpenAPI
         results: The results of this CredRevRecordDetailsResult [Optional].
     """
 
     results: Optional[List[IssuerCredRevRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[IssuerCredRevRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredRevRecordDetailsResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_rev_record_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_result.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.issuer_cred_rev_record import IssuerCredRevRecord
+from aries_cloudcontroller.model.issuer_rev_reg_record import IssuerRevRegRecord
 
 
-class CredRevRecordResult(BaseModel):
+class RevRegResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredRevRecordResult - a model defined in OpenAPI
-        result: The result of this CredRevRecordResult [Optional].
+    RevRegResult - a model defined in OpenAPI
+        result: The result of this RevRegResult [Optional].
     """
 
-    result: Optional[IssuerCredRevRecord] = None
-
-    def __init__(
-        self,
-        *,
-        result: Optional[IssuerCredRevRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
+    result: Optional[IssuerRevRegRecord] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredRevRecordResult.update_forward_refs()
+RevRegResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/cred_revoked_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_revoked_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     CredRevokedResult - a model defined in OpenAPI
         revoked: Whether credential is revoked on the ledger [Optional].
     """
 
     revoked: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        revoked: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            revoked=revoked,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredRevokedResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,39 +32,14 @@
     issuance_date: str = Field(..., alias="issuanceDate")
     issuer: Dict[str, Any]
     type: List[str]
     expiration_date: Optional[str] = Field(None, alias="expirationDate")
     id: Optional[str] = None
     proof: Optional[LinkedDataProof] = None
 
-    def __init__(
-        self,
-        *,
-        context: List[Dict] = None,
-        credential_subject: Dict[str, Any] = None,
-        issuance_date: str = None,
-        issuer: Dict[str, Any] = None,
-        type: List[str] = None,
-        expiration_date: Optional[str] = None,
-        id: Optional[str] = None,
-        proof: Optional[LinkedDataProof] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            context=context,
-            credential_subject=credential_subject,
-            expiration_date=expiration_date,
-            id=id,
-            issuance_date=issuance_date,
-            issuer=issuer,
-            proof=proof,
-            type=type,
-            **kwargs,
-        )
-
     @validator("expiration_date")
     def expiration_date_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([0-9]{4})-([0-9]{2})-([0-9]{2})([Tt ]([0-9]{2}):([0-9]{2}):([0-9]{2})(\.[0-9]+)?)?(([Zz]|([+-])([0-9]{2}):([0-9]{2})))?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,35 +28,14 @@
     id: Optional[str] = None
     schema_id: Optional[str] = Field(None, alias="schemaId")
     tag: Optional[str] = None
     type: Optional[Literal["CL"]] = None
     value: Optional[CredDefValue] = None
     ver: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        tag: Optional[str] = None,
-        type: Optional[Literal["CL"]] = None,
-        value: Optional[CredDefValue] = None,
-        ver: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            schema_id=schema_id,
-            tag=tag,
-            type=type,
-            value=value,
-            ver=ver,
-            **kwargs,
-        )
-
     @validator("id")
     def id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_get_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_get_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     CredentialDefinitionGetResult - a model defined in OpenAPI
         credential_definition: The credential_definition of this CredentialDefinitionGetResult [Optional].
     """
 
     credential_definition: Optional[CredentialDefinition] = None
 
-    def __init__(
-        self,
-        *,
-        credential_definition: Optional[CredentialDefinition] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_definition=credential_definition,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredentialDefinitionGetResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_send_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_send_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,31 +23,14 @@
     """
 
     revocation_registry_size: Optional[int] = None
     schema_id: Optional[str] = None
     support_revocation: Optional[bool] = None
     tag: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        revocation_registry_size: Optional[int] = None,
-        schema_id: Optional[str] = None,
-        support_revocation: Optional[bool] = None,
-        tag: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            revocation_registry_size=revocation_registry_size,
-            schema_id=schema_id,
-            support_revocation=support_revocation,
-            tag=tag,
-            **kwargs,
-        )
-
     @validator("revocation_registry_size")
     def revocation_registry_size_max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 32768:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definition_send_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_definition_send_result.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,25 +17,14 @@
 
     CredentialDefinitionSendResult - a model defined in OpenAPI
         credential_definition_id: Credential definition identifier [Optional].
     """
 
     credential_definition_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        credential_definition_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_definition_id=credential_definition_id,
-            **kwargs,
-        )
-
     @validator("credential_definition_id")
     def credential_definition_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_definitions_created_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_credential_definition_send_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,36 +4,31 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.credential_definition_send_result import (
+    CredentialDefinitionSendResult,
+)
+from aries_cloudcontroller.model.transaction_record import TransactionRecord
 
 
-class CredentialDefinitionsCreatedResult(BaseModel):
+class TxnOrCredentialDefinitionSendResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredentialDefinitionsCreatedResult - a model defined in OpenAPI
-        credential_definition_ids: The credential_definition_ids of this CredentialDefinitionsCreatedResult [Optional].
+    TxnOrCredentialDefinitionSendResult - a model defined in OpenAPI
+        sent: The sent of this TxnOrCredentialDefinitionSendResult [Optional].
+        txn: Credential definition transaction to endorse [Optional].
     """
 
-    credential_definition_ids: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        credential_definition_ids: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_definition_ids=credential_definition_ids,
-            **kwargs,
-        )
+    sent: Optional[CredentialDefinitionSendResult] = None
+    txn: Optional[TransactionRecord] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredentialDefinitionsCreatedResult.update_forward_refs()
+TxnOrCredentialDefinitionSendResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_offer.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_offer.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,31 +27,12 @@
 
     offersattach: List[AttachDecorator] = Field(..., alias="offers~attach")
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
     credential_preview: Optional[CredentialPreview] = None
 
-    def __init__(
-        self,
-        *,
-        offersattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[CredentialPreview] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            credential_preview=credential_preview,
-            offersattach=offersattach,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredentialOffer.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_preview.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_preview.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,12 @@
         attributes: The attributes of this CredentialPreview.
         type: Message type identifier [Optional].
     """
 
     attributes: List[CredAttrSpec]
     type: Optional[str] = Field(None, alias="@type")
 
-    def __init__(
-        self,
-        *,
-        attributes: List[CredAttrSpec] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            type=type,
-            attributes=attributes,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 CredentialPreview.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/credential_proposal.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,43 +36,14 @@
     credential_proposal: Optional[CredentialPreview] = None
     issuer_did: Optional[str] = None
     schema_id: Optional[str] = None
     schema_issuer_did: Optional[str] = None
     schema_name: Optional[str] = None
     schema_version: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        cred_def_id: Optional[str] = None,
-        credential_proposal: Optional[CredentialPreview] = None,
-        issuer_did: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        schema_issuer_did: Optional[str] = None,
-        schema_name: Optional[str] = None,
-        schema_version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            cred_def_id=cred_def_id,
-            credential_proposal=credential_proposal,
-            issuer_did=issuer_did,
-            schema_id=schema_id,
-            schema_issuer_did=schema_issuer_did,
-            schema_name=schema_name,
-            schema_version=schema_version,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/credential_status_options.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/disclose.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,36 +4,30 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.protocol_descriptor import ProtocolDescriptor
 
 
-class CredentialStatusOptions(BaseModel):
+class Disclose(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    CredentialStatusOptions - a model defined in OpenAPI
-        type: Credential status method type to use for the credential. Should match status method registered in the Verifiable Credential Extension Registry.
+    Disclose - a model defined in OpenAPI
+        protocols: List of protocol descriptors.
+        id: Message identifier [Optional].
+        type: Message type [Optional].
     """
 
-    type: str
-
-    def __init__(
-        self,
-        *,
-        type: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            type=type,
-            **kwargs,
-        )
+    protocols: List[ProtocolDescriptor]
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
 
     class Config:
         allow_population_by_field_name = True
 
 
-CredentialStatusOptions.update_forward_refs()
+Disclose.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/date.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query_paginate.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class Date(BaseModel):
+class KeylistQueryPaginate(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Date - a model defined in OpenAPI
-        expires_time: Expiry Date.
+    KeylistQueryPaginate - a model defined in OpenAPI
+        limit: Limit for keylist query [Optional].
+        offset: Offset value for query [Optional].
     """
 
-    expires_time: datetime
-
-    def __init__(
-        self,
-        *,
-        expires_time: datetime = None,
-        **kwargs,
-    ):
-        super().__init__(
-            expires_time=expires_time,
-            **kwargs,
-        )
+    limit: Optional[int] = None
+    offset: Optional[int] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Date.update_forward_refs()
+KeylistQueryPaginate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,33 +25,14 @@
 
     did: Optional[str] = None
     key_type: Optional[Literal["ed25519", "bls12381g2"]] = None
     method: Optional[Literal["sov", "key"]] = None
     posture: Optional[Literal["public", "posted", "wallet_only"]] = None
     verkey: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        did: Optional[str] = None,
-        key_type: Optional[Literal["ed25519", "bls12381g2"]] = None,
-        method: Optional[Literal["sov", "key"]] = None,
-        posture: Optional[Literal["public", "posted", "wallet_only"]] = None,
-        verkey: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            did=did,
-            key_type=key_type,
-            method=method,
-            posture=posture,
-            verkey=verkey,
-            **kwargs,
-        )
-
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_create.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,27 +22,12 @@
         seed: Optional seed to use for DID, Must beenabled in configuration before use. [Optional].
     """
 
     method: Optional[Literal["key", "sov"]] = None
     options: Optional[DIDCreateOptions] = None
     seed: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        method: Optional[Literal["key", "sov"]] = None,
-        options: Optional[DIDCreateOptions] = None,
-        seed: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            method=method,
-            options=options,
-            seed=seed,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 DIDCreate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_create_options.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_create_options.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         key_type: Key type to use for the DID keypair. Validated with the chosen DID method's supported key types..
         did: Specify final value of the did (including did:&lt;method&gt;: prefix)if the method supports or requires so. [Optional].
     """
 
     key_type: Literal["ed25519", "bls12381g2"]
     did: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        key_type: Literal["ed25519", "bls12381g2"] = None,
-        did: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            did=did,
-            key_type=key_type,
-            **kwargs,
-        )
-
     @validator("did")
     def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$|^did:([a-zA-Z0-9_]+):([a-zA-Z0-9_.%-]+(:[a-zA-Z0-9_.%-]+)*)((;[a-zA-Z0-9_.:%-]+=[a-zA-Z0-9_.:%-]*)*)(\\/[^#?]*)?([?][^#]*)?(\#.*)?$$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_endpoint.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/did_endpoint_with_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,39 +6,28 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class DIDEndpoint(BaseModel):
+class DIDEndpointWithType(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDEndpoint - a model defined in OpenAPI
+    DIDEndpointWithType - a model defined in OpenAPI
         did: DID of interest.
         endpoint: Endpoint to set (omit to delete) [Optional].
+        endpoint_type: Endpoint type to set (default &#39;Endpoint&#39;); affects only public or posted DIDs [Optional].
     """
 
     did: str
     endpoint: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        did: str = None,
-        endpoint: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            did=did,
-            endpoint=endpoint,
-            **kwargs,
-        )
+    endpoint_type: Optional[Literal["Endpoint", "Profile", "LinkedDomains"]] = None
 
     @validator("did")
     def did_pattern(cls, value):
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
         return value
@@ -56,8 +45,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDEndpoint.update_forward_refs()
+DIDEndpointWithType.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_endpoint_with_type.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/wallet_record.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,62 +6,59 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class DIDEndpointWithType(BaseModel):
+class WalletRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDEndpointWithType - a model defined in OpenAPI
-        did: DID of interest.
-        endpoint: Endpoint to set (omit to delete) [Optional].
-        endpoint_type: Endpoint type to set (default &#39;Endpoint&#39;); affects only public or posted DIDs [Optional].
+    WalletRecord - a model defined in OpenAPI
+        key_management_mode: Mode regarding management of wallet key.
+        wallet_id: Wallet record ID.
+        created_at: Time of record creation [Optional].
+        settings: Settings for this wallet. [Optional].
+        state: Current record state [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
-    did: str
-    endpoint: Optional[str] = None
-    endpoint_type: Optional[Literal["Endpoint", "Profile", "LinkedDomains"]] = None
-
-    def __init__(
-        self,
-        *,
-        did: str = None,
-        endpoint: Optional[str] = None,
-        endpoint_type: Optional[Literal["Endpoint", "Profile", "LinkedDomains"]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            did=did,
-            endpoint=endpoint,
-            endpoint_type=endpoint_type,
-            **kwargs,
-        )
-
-    @validator("did")
-    def did_pattern(cls, value):
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+    key_management_mode: Literal["managed", "unmanaged"]
+    wallet_id: str
+    created_at: Optional[str] = None
+    settings: Optional[Dict[str, Any]] = None
+    state: Optional[str] = None
+    updated_at: Optional[str] = None
+
+    @validator("created_at")
+    def created_at_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
+            raise ValueError(
+                f"Value of created_at does not match regex pattern ('{pattern}')"
+            )
         return value
 
-    @validator("endpoint")
-    def endpoint_pattern(cls, value):
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[A-Za-z0-9\.\-\+]+:\/\/([A-Za-z0-9][.A-Za-z0-9-_]+[A-Za-z0-9])+(:[1-9][0-9]*)?(\/[^?&#]+)?$"
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of endpoint does not match regex pattern ('{pattern}')"
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDEndpointWithType.update_forward_refs()
+WalletRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_holder.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.did import DID
 
 
-class DIDList(BaseModel):
+class DIFHolder(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDList - a model defined in OpenAPI
-        results: DID list [Optional].
+    DIFHolder - a model defined in OpenAPI
+        directive: Preference [Optional].
+        field_id: The field_id of this DIFHolder [Optional].
     """
 
-    results: Optional[List[DID]] = None
-
-    def __init__(
-        self,
-        *,
-        results: Optional[List[DID]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
+    directive: Optional[Literal["required", "preferred"]] = None
+    field_id: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDList.update_forward_refs()
+DIFHolder.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/did_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,37 +4,25 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.did import DID
 
 
-class DIDResult(BaseModel):
+class RevRegUpdateTailsFileUri(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDResult - a model defined in OpenAPI
-        result: The result of this DIDResult [Optional].
+    RevRegUpdateTailsFileUri - a model defined in OpenAPI
+        tails_public_uri: Public URI to the tails file.
     """
 
-    result: Optional[DID] = None
-
-    def __init__(
-        self,
-        *,
-        result: Optional[DID] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
+    tails_public_uri: str
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDResult.update_forward_refs()
+RevRegUpdateTailsFileUri.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/didx_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,61 +7,39 @@
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
 
 
-class DIDXRequest(BaseModel):
+class InvitationMessage(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIDXRequest - a model defined in OpenAPI
-        label: Label for DID exchange request.
+    InvitationMessage - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
-        did: DID of exchange [Optional].
-        did_docattach: As signed attachment, DID Doc associated with DID [Optional].
+        accept: List of mime type in order of preference [Optional].
+        handshake_protocols: The handshake_protocols of this InvitationMessage [Optional].
+        image_url: Optional image URL for out-of-band invitation [Optional].
+        label: Optional label [Optional].
+        requestsattach: Optional request attachment [Optional].
+        services: The services of this InvitationMessage [Optional].
     """
 
-    label: str
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
-    did: Optional[str] = None
-    did_docattach: Optional[AttachDecorator] = Field(None, alias="did_doc~attach")
-
-    def __init__(
-        self,
-        *,
-        label: str = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        did: Optional[str] = None,
-        did_docattach: Optional[AttachDecorator] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            did=did,
-            did_docattach=did_docattach,
-            label=label,
-            **kwargs,
-        )
-
-    @validator("did")
-    def did_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
-        if not re.match(pattern, value):
-            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
-        return value
+    accept: Optional[List[str]] = None
+    handshake_protocols: Optional[List[str]] = None
+    image_url: Optional[str] = Field(None, alias="imageUrl")
+    label: Optional[str] = None
+    requestsattach: Optional[List[AttachDecorator]] = Field(
+        None, alias="requests~attach"
+    )
+    services: Optional[List[Union[Dict, str]]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIDXRequest.update_forward_refs()
+InvitationMessage.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_field.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,53 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.filter import Filter
+from aries_cloudcontroller.model.menu_option import MenuOption
 
 
-class DIFField(BaseModel):
+class Menu(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIFField - a model defined in OpenAPI
-        filter: The filter of this DIFField [Optional].
-        id: ID [Optional].
-        path: The path of this DIFField [Optional].
-        predicate: Preference [Optional].
-        purpose: Purpose [Optional].
+    Menu - a model defined in OpenAPI
+        options: List of menu options.
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        description: Introductory text for the menu [Optional].
+        errormsg: An optional error message to display in menu header [Optional].
+        title: Menu title [Optional].
     """
 
-    filter: Optional[Filter] = None
-    id: Optional[str] = None
-    path: Optional[List[str]] = None
-    predicate: Optional[Literal["required", "preferred"]] = None
-    purpose: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        filter: Optional[Filter] = None,
-        id: Optional[str] = None,
-        path: Optional[List[str]] = None,
-        predicate: Optional[Literal["required", "preferred"]] = None,
-        purpose: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            filter=filter,
-            id=id,
-            path=path,
-            predicate=predicate,
-            purpose=purpose,
-            **kwargs,
-        )
+    options: List[MenuOption]
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    description: Optional[str] = None
+    errormsg: Optional[str] = None
+    title: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIFField.update_forward_refs()
+Menu.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_holder.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_ge_proof_pred.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,38 +6,27 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class DIFHolder(BaseModel):
+class IndyGEProofPred(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    DIFHolder - a model defined in OpenAPI
-        directive: Preference [Optional].
-        field_id: The field_id of this DIFHolder [Optional].
+    IndyGEProofPred - a model defined in OpenAPI
+        attr_name: Attribute name, indy-canonicalized [Optional].
+        p_type: Predicate type [Optional].
+        value: Predicate threshold value [Optional].
     """
 
-    directive: Optional[Literal["required", "preferred"]] = None
-    field_id: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        directive: Optional[Literal["required", "preferred"]] = None,
-        field_id: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            directive=directive,
-            field_id=field_id,
-            **kwargs,
-        )
+    attr_name: Optional[str] = None
+    p_type: Optional[Literal["LT", "LE", "GE", "GT"]] = None
+    value: Optional[int] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-DIFHolder.update_forward_refs()
+IndyGEProofPred.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_options.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         challenge: Challenge protect against replay attack [Optional].
         domain: Domain protect against replay attack [Optional].
     """
 
     challenge: Optional[str] = None
     domain: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        challenge: Optional[str] = None,
-        domain: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            challenge=challenge,
-            domain=domain,
-            **kwargs,
-        )
-
     @validator("challenge")
     def challenge_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-4[a-fA-F0-9]{3}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_pres_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_pres_spec.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,29 +24,12 @@
     """
 
     issuer_id: Optional[str] = None
     presentation_definition: Optional[PresentationDefinition] = None
     record_ids: Optional[Dict[str, Any]] = None
     reveal_doc: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        issuer_id: Optional[str] = None,
-        presentation_definition: Optional[PresentationDefinition] = None,
-        record_ids: Optional[Dict[str, Any]] = None,
-        reveal_doc: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            issuer_id=issuer_id,
-            presentation_definition=presentation_definition,
-            record_ids=record_ids,
-            reveal_doc=reveal_doc,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 DIFPresSpec.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_proof_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_proof_proposal.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         input_descriptors: The input_descriptors of this DIFProofProposal [Optional].
         options: The options of this DIFProofProposal [Optional].
     """
 
     input_descriptors: Optional[List[InputDescriptors]] = None
     options: Optional[DIFOptions] = None
 
-    def __init__(
-        self,
-        *,
-        input_descriptors: Optional[List[InputDescriptors]] = None,
-        options: Optional[DIFOptions] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            input_descriptors=input_descriptors,
-            options=options,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 DIFProofProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/dif_proof_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/dif_proof_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         presentation_definition: The presentation_definition of this DIFProofRequest.
         options: The options of this DIFProofRequest [Optional].
     """
 
     presentation_definition: PresentationDefinition
     options: Optional[DIFOptions] = None
 
-    def __init__(
-        self,
-        *,
-        presentation_definition: PresentationDefinition = None,
-        options: Optional[DIFOptions] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            options=options,
-            presentation_definition=presentation_definition,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 DIFProofRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/disclose.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_form.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,45 +4,32 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.protocol_descriptor import ProtocolDescriptor
+from aries_cloudcontroller.model.menu_form_param import MenuFormParam
 
 
-class Disclose(BaseModel):
+class MenuForm(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Disclose - a model defined in OpenAPI
-        protocols: List of protocol descriptors.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
+    MenuForm - a model defined in OpenAPI
+        description: Additional descriptive text for menu form [Optional].
+        params: List of form parameters [Optional].
+        submit_label: Alternative label for form submit button [Optional].
+        title: Menu form title [Optional].
     """
 
-    protocols: List[ProtocolDescriptor]
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
-
-    def __init__(
-        self,
-        *,
-        protocols: List[ProtocolDescriptor] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            protocols=protocols,
-            **kwargs,
-        )
+    description: Optional[str] = None
+    params: Optional[List[MenuFormParam]] = None
+    submit_label: Optional[str] = Field(None, alias="submit-label")
+    title: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Disclose.update_forward_refs()
+MenuForm.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/disclosures.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/disclosures.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         type: Message type [Optional].
     """
 
     disclosures: List[Dict]
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
 
-    def __init__(
-        self,
-        *,
-        disclosures: List[Dict] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            disclosures=disclosures,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 Disclosures.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/doc.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/doc.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,12 @@
         credential: Credential to sign.
         options: Signature options.
     """
 
     credential: Dict[str, Any]
     options: SignatureOptions
 
-    def __init__(
-        self,
-        *,
-        credential: Dict[str, Any] = None,
-        options: SignatureOptions = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential=credential,
-            options=options,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 Doc.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/endorser_info.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/write_ledger_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,38 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class EndorserInfo(BaseModel):
+class WriteLedgerRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    EndorserInfo - a model defined in OpenAPI
-        endorser_did: Endorser DID.
-        endorser_name: Endorser Name [Optional].
+    WriteLedgerRequest - a model defined in OpenAPI
+        ledger_id: The ledger_id of this WriteLedgerRequest [Optional].
     """
 
-    endorser_did: str
-    endorser_name: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        endorser_did: str = None,
-        endorser_name: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            endorser_did=endorser_did,
-            endorser_name=endorser_name,
-            **kwargs,
-        )
+    ledger_id: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-EndorserInfo.update_forward_refs()
+WriteLedgerRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/endpoints_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/endpoints_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         my_endpoint: My endpoint [Optional].
         their_endpoint: Their endpoint [Optional].
     """
 
     my_endpoint: Optional[str] = None
     their_endpoint: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        my_endpoint: Optional[str] = None,
-        their_endpoint: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            my_endpoint=my_endpoint,
-            their_endpoint=their_endpoint,
-            **kwargs,
-        )
-
     @validator("my_endpoint")
     def my_endpoint_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[A-Za-z0-9\.\-\+]+:\/\/([A-Za-z0-9][.A-Za-z0-9-_]+[A-Za-z0-9])+(:[1-9][0-9]*)?(\/[^?&#]+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/generated.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/linked_data_proof.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,81 +6,70 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class Generated(BaseModel):
+class LinkedDataProof(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Generated - a model defined in OpenAPI
-        master_secret: The master_secret of this Generated [Optional].
-        number: The number of this Generated [Optional].
-        remainder: The remainder of this Generated [Optional].
+    LinkedDataProof - a model defined in OpenAPI
+        created: The string value of an ISO8601 combined date and time string generated by the Signature Algorithm.
+        proof_purpose: Proof purpose.
+        type: Identifies the digital signature suite that was used to create the signature.
+        verification_method: Information used for proof verification.
+        challenge: Associates a challenge with a proof, for use with a proofPurpose such as authentication [Optional].
+        domain: A string value specifying the restricted domain of the signature. [Optional].
+        jws: Associates a Detached Json Web Signature with a proof [Optional].
+        nonce: The nonce [Optional].
+        proof_value: The proof value of a proof [Optional].
     """
 
-    master_secret: Optional[str] = None
-    number: Optional[str] = None
-    remainder: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        master_secret: Optional[str] = None,
-        number: Optional[str] = None,
-        remainder: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            master_secret=master_secret,
-            number=number,
-            remainder=remainder,
-            **kwargs,
-        )
-
-    @validator("master_secret")
-    def master_secret_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^[0-9]*$"
+    created: str
+    proof_purpose: str = Field(..., alias="proofPurpose")
+    type: str
+    verification_method: str = Field(..., alias="verificationMethod")
+    challenge: Optional[str] = None
+    domain: Optional[str] = None
+    jws: Optional[str] = None
+    nonce: Optional[str] = None
+    proof_value: Optional[str] = Field(None, alias="proofValue")
+
+    @validator("created")
+    def created_pattern(cls, value):
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of master_secret does not match regex pattern ('{pattern}')"
+                f"Value of created does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("number")
-    def number_pattern(cls, value):
+    @validator("domain")
+    def domain_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[0-9]*$"
+        pattern = r"\w+:(\\/?\\/?)[^\s]+"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of number does not match regex pattern ('{pattern}')"
+                f"Value of domain does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("remainder")
-    def remainder_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^[0-9]*$"
+    @validator("verification_method")
+    def verification_method_pattern(cls, value):
+        pattern = r"\w+:(\\/?\\/?)[^\s]+"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of remainder does not match regex pattern ('{pattern}')"
+                f"Value of verification_method does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-Generated.update_forward_refs()
+LinkedDataProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_did_endpoint_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_did_endpoint_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,25 +17,14 @@
 
     GetDIDEndpointResponse - a model defined in OpenAPI
         endpoint: Full verification key [Optional].
     """
 
     endpoint: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        endpoint: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            endpoint=endpoint,
-            **kwargs,
-        )
-
     @validator("endpoint")
     def endpoint_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[A-Za-z0-9\.\-\+]+:\/\/([A-Za-z0-9][.A-Za-z0-9-_]+[A-Za-z0-9])+(:[1-9][0-9]*)?(\/[^?&#]+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_did_verkey_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_did_verkey_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,25 +17,14 @@
 
     GetDIDVerkeyResponse - a model defined in OpenAPI
         verkey: Full verification key [Optional].
     """
 
     verkey: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        verkey: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            verkey=verkey,
-            **kwargs,
-        )
-
     @validator("verkey")
     def verkey_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = (
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/get_nym_role_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/get_nym_role_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,32 +21,12 @@
 
     role: Optional[
         Literal[
             "STEWARD", "TRUSTEE", "ENDORSER", "NETWORK_MONITOR", "USER", "ROLE_REMOVE"
         ]
     ] = None
 
-    def __init__(
-        self,
-        *,
-        role: Optional[
-            Literal[
-                "STEWARD",
-                "TRUSTEE",
-                "ENDORSER",
-                "NETWORK_MONITOR",
-                "USER",
-                "ROLE_REMOVE",
-            ]
-        ] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            role=role,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 GetNymRoleResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_abstract.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,31 +26,14 @@
     """
 
     cred_def_id: str
     key_correctness_proof: IndyKeyCorrectnessProof
     nonce: str
     schema_id: str
 
-    def __init__(
-        self,
-        *,
-        cred_def_id: str = None,
-        key_correctness_proof: IndyKeyCorrectnessProof = None,
-        nonce: str = None,
-        schema_id: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            key_correctness_proof=key_correctness_proof,
-            nonce=nonce,
-            schema_id=schema_id,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of cred_def_id does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_info.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,35 +27,14 @@
     attrs: Optional[Dict[str, str]] = None
     cred_def_id: Optional[str] = None
     cred_rev_id: Optional[str] = None
     referent: Optional[str] = None
     rev_reg_id: Optional[str] = None
     schema_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        attrs: Optional[Dict[str, str]] = None,
-        cred_def_id: Optional[str] = None,
-        cred_rev_id: Optional[str] = None,
-        referent: Optional[str] = None,
-        rev_reg_id: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attrs=attrs,
-            cred_def_id=cred_def_id,
-            cred_rev_id=cred_rev_id,
-            referent=referent,
-            rev_reg_id=rev_reg_id,
-            schema_id=schema_id,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_precis.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_precis.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,27 +25,12 @@
         presentation_referents: The presentation_referents of this IndyCredPrecis [Optional].
     """
 
     cred_info: Optional[IndyCredInfo] = None
     interval: Optional[IndyNonRevocationInterval] = None
     presentation_referents: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        cred_info: Optional[IndyCredInfo] = None,
-        interval: Optional[IndyNonRevocationInterval] = None,
-        presentation_referents: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_info=cred_info,
-            interval=interval,
-            presentation_referents=presentation_referents,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyCredPrecis.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_cred_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_cred_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,33 +25,14 @@
 
     blinded_ms: Dict[str, Any]
     blinded_ms_correctness_proof: Dict[str, Any]
     cred_def_id: str
     nonce: str
     prover_did: str
 
-    def __init__(
-        self,
-        *,
-        blinded_ms: Dict[str, Any] = None,
-        blinded_ms_correctness_proof: Dict[str, Any] = None,
-        cred_def_id: str = None,
-        nonce: str = None,
-        prover_did: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            blinded_ms=blinded_ms,
-            blinded_ms_correctness_proof=blinded_ms_correctness_proof,
-            cred_def_id=cred_def_id,
-            nonce=nonce,
-            prover_did=prover_did,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of cred_def_id does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_credential.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_indy.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,73 +4,66 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.indy_attr_value import IndyAttrValue
 
 
-class IndyCredential(BaseModel):
+class V20CredExRecordIndy(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyCredential - a model defined in OpenAPI
-        cred_def_id: Credential definition identifier.
-        schema_id: Schema identifier.
-        signature: Credential signature.
-        signature_correctness_proof: Credential signature correctness proof.
-        values: Credential attributes.
-        rev_reg: Revocation registry state [Optional].
+    V20CredExRecordIndy - a model defined in OpenAPI
+        created_at: Time of record creation [Optional].
+        cred_ex_id: Corresponding v2.0 credential exchange record identifier [Optional].
+        cred_ex_indy_id: Record identifier [Optional].
+        cred_id_stored: Credential identifier stored in wallet [Optional].
+        cred_request_metadata: Credential request metadata for indy holder [Optional].
+        cred_rev_id: Credential revocation identifier within revocation registry [Optional].
         rev_reg_id: Revocation registry identifier [Optional].
-        witness: Witness for revocation proof [Optional].
+        state: Current record state [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
-    cred_def_id: str
-    schema_id: str
-    signature: Dict[str, Any]
-    signature_correctness_proof: Dict[str, Any]
-    values: Dict[str, IndyAttrValue]
-    rev_reg: Optional[Dict[str, Any]] = None
+    created_at: Optional[str] = None
+    cred_ex_id: Optional[str] = None
+    cred_ex_indy_id: Optional[str] = None
+    cred_id_stored: Optional[str] = None
+    cred_request_metadata: Optional[Dict[str, Any]] = None
+    cred_rev_id: Optional[str] = None
     rev_reg_id: Optional[str] = None
-    witness: Optional[Dict[str, Any]] = None
+    state: Optional[str] = None
+    updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        cred_def_id: str = None,
-        schema_id: str = None,
-        signature: Dict[str, Any] = None,
-        signature_correctness_proof: Dict[str, Any] = None,
-        values: Dict[str, IndyAttrValue] = None,
-        rev_reg: Optional[Dict[str, Any]] = None,
-        rev_reg_id: Optional[str] = None,
-        witness: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            rev_reg=rev_reg,
-            rev_reg_id=rev_reg_id,
-            schema_id=schema_id,
-            signature=signature,
-            signature_correctness_proof=signature_correctness_proof,
-            values=values,
-            witness=witness,
-            **kwargs,
-        )
-
-    @validator("cred_def_id")
-    def cred_def_id_pattern(cls, value):
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
+    @validator("created_at")
+    def created_at_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
+                f"Value of created_at does not match regex pattern ('{pattern}')"
+            )
+        return value
+
+    @validator("cred_rev_id")
+    def cred_rev_id_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[1-9][0-9]*$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of cred_rev_id does not match regex pattern ('{pattern}')"
             )
         return value
 
     @validator("rev_reg_id")
     def rev_reg_id_pattern(cls, value):
         # Property is optional
         if value is None:
@@ -79,21 +72,25 @@
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of rev_reg_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("schema_id")
-    def schema_id_pattern(cls, value):
-        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of schema_id does not match regex pattern ('{pattern}')"
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyCredential.update_forward_refs()
+V20CredExRecordIndy.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_eq_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_eq_proof.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,35 +27,14 @@
     a_prime: Optional[str] = None
     e: Optional[str] = None
     m: Optional[Dict[str, str]] = None
     m2: Optional[str] = None
     revealed_attrs: Optional[Dict[str, str]] = None
     v: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        a_prime: Optional[str] = None,
-        e: Optional[str] = None,
-        m: Optional[Dict[str, str]] = None,
-        m2: Optional[str] = None,
-        revealed_attrs: Optional[Dict[str, str]] = None,
-        v: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            a_prime=a_prime,
-            e=e,
-            m=m,
-            m2=m2,
-            revealed_attrs=revealed_attrs,
-            v=v,
-            **kwargs,
-        )
-
     @validator("a_prime")
     def a_prime_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_ge_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/cred_def_value_primary.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,81 +4,80 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.indy_ge_proof_pred import IndyGEProofPred
+from aries_cloudcontroller.model.generated import Generated
 
 
-class IndyGEProof(BaseModel):
+class CredDefValuePrimary(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyGEProof - a model defined in OpenAPI
-        alpha: The alpha of this IndyGEProof [Optional].
-        mj: The mj of this IndyGEProof [Optional].
-        predicate: The predicate of this IndyGEProof [Optional].
-        r: The r of this IndyGEProof [Optional].
-        t: The t of this IndyGEProof [Optional].
-        u: The u of this IndyGEProof [Optional].
+    CredDefValuePrimary - a model defined in OpenAPI
+        n: The n of this CredDefValuePrimary [Optional].
+        r: The r of this CredDefValuePrimary [Optional].
+        rctxt: The rctxt of this CredDefValuePrimary [Optional].
+        s: The s of this CredDefValuePrimary [Optional].
+        z: The z of this CredDefValuePrimary [Optional].
     """
 
-    alpha: Optional[str] = None
-    mj: Optional[str] = None
-    predicate: Optional[IndyGEProofPred] = None
-    r: Optional[Dict[str, str]] = None
-    t: Optional[Dict[str, str]] = None
-    u: Optional[Dict[str, str]] = None
-
-    def __init__(
-        self,
-        *,
-        alpha: Optional[str] = None,
-        mj: Optional[str] = None,
-        predicate: Optional[IndyGEProofPred] = None,
-        r: Optional[Dict[str, str]] = None,
-        t: Optional[Dict[str, str]] = None,
-        u: Optional[Dict[str, str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            alpha=alpha,
-            mj=mj,
-            predicate=predicate,
-            r=r,
-            t=t,
-            u=u,
-            **kwargs,
-        )
+    n: Optional[str] = None
+    r: Optional[Generated] = None
+    rctxt: Optional[str] = None
+    s: Optional[str] = None
+    z: Optional[str] = None
 
-    @validator("alpha")
-    def alpha_pattern(cls, value):
+    @validator("n")
+    def n_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[0-9]*$"
+        if not re.match(pattern, value):
+            raise ValueError(f"Value of n does not match regex pattern ('{pattern}')")
+        return value
+
+    @validator("rctxt")
+    def rctxt_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of alpha does not match regex pattern ('{pattern}')"
+                f"Value of rctxt does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("mj")
-    def mj_pattern(cls, value):
+    @validator("s")
+    def s_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[0-9]*$"
+        if not re.match(pattern, value):
+            raise ValueError(f"Value of s does not match regex pattern ('{pattern}')")
+        return value
+
+    @validator("z")
+    def z_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of mj does not match regex pattern ('{pattern}')")
+            raise ValueError(f"Value of z does not match regex pattern ('{pattern}')")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyGEProof.update_forward_refs()
+CredDefValuePrimary.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_ge_proof_pred.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/attach_decorator.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,44 +4,51 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.attach_decorator_data import AttachDecoratorData
 
 
-class IndyGEProofPred(BaseModel):
+class AttachDecorator(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyGEProofPred - a model defined in OpenAPI
-        attr_name: Attribute name, indy-canonicalized [Optional].
-        p_type: Predicate type [Optional].
-        value: Predicate threshold value [Optional].
+    AttachDecorator - a model defined in OpenAPI
+        data: The data of this AttachDecorator.
+        id: Attachment identifier [Optional].
+        byte_count: Byte count of data included by reference [Optional].
+        description: Human-readable description of content [Optional].
+        filename: File name [Optional].
+        lastmod_time: Hint regarding last modification datetime, in ISO-8601 format [Optional].
+        mime_type: MIME type [Optional].
     """
 
-    attr_name: Optional[str] = None
-    p_type: Optional[Literal["LT", "LE", "GE", "GT"]] = None
-    value: Optional[int] = None
-
-    def __init__(
-        self,
-        *,
-        attr_name: Optional[str] = None,
-        p_type: Optional[Literal["LT", "LE", "GE", "GT"]] = None,
-        value: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attr_name=attr_name,
-            p_type=p_type,
-            value=value,
-            **kwargs,
-        )
+    data: AttachDecoratorData
+    id: Optional[str] = Field(None, alias="@id")
+    byte_count: Optional[int] = None
+    description: Optional[str] = None
+    filename: Optional[str] = None
+    lastmod_time: Optional[str] = None
+    mime_type: Optional[str] = Field(None, alias="mime-type")
+
+    @validator("lastmod_time")
+    def lastmod_time_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of lastmod_time does not match regex pattern ('{pattern}')"
+            )
+        return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyGEProofPred.update_forward_refs()
+AttachDecorator.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_key_correctness_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_key_correctness_proof.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,29 +21,14 @@
         xz_cap: xz_cap in key correctness proof.
     """
 
     c: str
     xr_cap: List[List[str]]
     xz_cap: str
 
-    def __init__(
-        self,
-        *,
-        c: str = None,
-        xr_cap: List[List[str]] = None,
-        xz_cap: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            c=c,
-            xr_cap=xr_cap,
-            xz_cap=xz_cap,
-            **kwargs,
-        )
-
     @validator("c")
     def c_pattern(cls, value):
         pattern = r"^[0-9]*$"
         if not re.match(pattern, value):
             raise ValueError(f"Value of c does not match regex pattern ('{pattern}')")
         return value
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_non_revoc_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_non_revoc_proof.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         c_list: The c_list of this IndyNonRevocProof [Optional].
         x_list: The x_list of this IndyNonRevocProof [Optional].
     """
 
     c_list: Optional[Dict[str, str]] = None
     x_list: Optional[Dict[str, str]] = None
 
-    def __init__(
-        self,
-        *,
-        c_list: Optional[Dict[str, str]] = None,
-        x_list: Optional[Dict[str, str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            c_list=c_list,
-            x_list=x_list,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyNonRevocProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_non_revocation_interval.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_non_revocation_interval.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         from_: Earliest time of interest in non-revocation interval [Optional].
         to: Latest time of interest in non-revocation interval [Optional].
     """
 
     from_: Optional[int] = Field(None, alias="from")
     to: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        from_: Optional[int] = None,
-        to: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            from_=from_,
-            to=to,
-            **kwargs,
-        )
-
     @validator("from_")
     def from__max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 18446744073709551615:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_attr_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_attr_spec.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,33 +25,14 @@
 
     name: str
     cred_def_id: Optional[str] = None
     mime_type: Optional[str] = Field(None, alias="mime-type")
     referent: Optional[str] = None
     value: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        name: str = None,
-        cred_def_id: Optional[str] = None,
-        mime_type: Optional[str] = None,
-        referent: Optional[str] = None,
-        value: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            mime_type=mime_type,
-            name=name,
-            referent=referent,
-            value=value,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_pred_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_pred_spec.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,31 +23,14 @@
     """
 
     name: str
     predicate: Literal["<", "<=", ">=", ">"]
     threshold: int
     cred_def_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        name: str = None,
-        predicate: Literal["<", "<=", ">=", ">"] = None,
-        threshold: int = None,
-        cred_def_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            name=name,
-            predicate=predicate,
-            threshold=threshold,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_pres_preview.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_pres_preview.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,27 +23,12 @@
         type: Message type identifier [Optional].
     """
 
     attributes: List[IndyPresAttrSpec]
     predicates: List[IndyPresPredSpec]
     type: Optional[str] = Field(None, alias="@type")
 
-    def __init__(
-        self,
-        *,
-        attributes: List[IndyPresAttrSpec] = None,
-        predicates: List[IndyPresPredSpec] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            type=type,
-            attributes=attributes,
-            predicates=predicates,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyPresPreview.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_primary_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_primary_proof.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         eq_proof: Indy equality proof [Optional].
         ge_proofs: Indy GE proofs [Optional].
     """
 
     eq_proof: Optional[IndyEQProof] = None
     ge_proofs: Optional[List[IndyGEProof]] = None
 
-    def __init__(
-        self,
-        *,
-        eq_proof: Optional[IndyEQProof] = None,
-        ge_proofs: Optional[List[IndyGEProof]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            eq_proof=eq_proof,
-            ge_proofs=ge_proofs,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyPrimaryProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_identifier.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/issuer_cred_rev_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,109 @@
 # coding: utf-8
 
 from __future__ import annotations
 
-import re  # noqa: F401
 from datetime import date, datetime  # noqa: F401
-from typing import Any, Dict, List, Literal, Optional, Union  # noqa: F401
 
-from pydantic import AnyUrl, BaseModel, EmailStr, Extra, Field, validator  # noqa: F401
+import re  # noqa: F401
+from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
+
+from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyProofIdentifier(BaseModel):
+class IssuerCredRevRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofIdentifier - a model defined in OpenAPI
+    IssuerCredRevRecord - a model defined in OpenAPI
+        created_at: Time of record creation [Optional].
         cred_def_id: Credential definition identifier [Optional].
+        cred_ex_id: Credential exchange record identifier at credential issue [Optional].
+        cred_ex_version: Credential exchange version [Optional].
+        cred_rev_id: Credential revocation identifier [Optional].
+        record_id: Issuer credential revocation record identifier [Optional].
         rev_reg_id: Revocation registry identifier [Optional].
-        schema_id: Schema identifier [Optional].
-        timestamp: Timestamp epoch [Optional].
+        state: Issue credential revocation record state [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
+    created_at: Optional[str] = None
     cred_def_id: Optional[str] = None
+    cred_ex_id: Optional[str] = None
+    cred_ex_version: Optional[str] = None
+    cred_rev_id: Optional[str] = None
+    record_id: Optional[str] = None
     rev_reg_id: Optional[str] = None
-    schema_id: Optional[str] = None
-    timestamp: Optional[int] = None
+    state: Optional[str] = None
+    updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        cred_def_id: Optional[str] = None,
-        rev_reg_id: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        timestamp: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            rev_reg_id=rev_reg_id,
-            schema_id=schema_id,
-            timestamp=timestamp,
-            **kwargs,
-        )
-
-    @validator("cred_def_id")
-    def cred_def_id_pattern(cls, value):
+    @validator("created_at")
+    def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
+                f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("rev_reg_id")
-    def rev_reg_id_pattern(cls, value):
+    @validator("cred_def_id")
+    def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
+        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of rev_reg_id does not match regex pattern ('{pattern}')"
+                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("schema_id")
-    def schema_id_pattern(cls, value):
+    @validator("cred_rev_id")
+    def cred_rev_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+        pattern = r"^[1-9][0-9]*$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of schema_id does not match regex pattern ('{pattern}')"
+                f"Value of cred_rev_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("timestamp")
-    def timestamp_max(cls, value):
+    @validator("rev_reg_id")
+    def rev_reg_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value > 18446744073709551615:
+        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
+        if not re.match(pattern, value):
             raise ValueError(
-                f"timestamp must be less than 18446744073709551615, currently {value}"
+                f"Value of rev_reg_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("timestamp")
-    def timestamp_min(cls, value):
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value < 0:
-            raise ValueError(f"timestamp must be greater than 0, currently {value}")
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
+            )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofIdentifier.update_forward_refs()
+IssuerCredRevRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,25 +25,12 @@
         aggregated_proof: Indy proof aggregated proof [Optional].
         proofs: Indy proof proofs [Optional].
     """
 
     aggregated_proof: Optional[IndyProofProofAggregatedProof] = None
     proofs: Optional[List[IndyProofProofProofsProof]] = None
 
-    def __init__(
-        self,
-        *,
-        aggregated_proof: Optional[IndyProofProofAggregatedProof] = None,
-        proofs: Optional[List[IndyProofProofProofsProof]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            aggregated_proof=aggregated_proof,
-            proofs=proofs,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof_aggregated_proof.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         c_hash: c_hash value [Optional].
         c_list: c_list value [Optional].
     """
 
     c_hash: Optional[str] = None
     c_list: Optional[List[List[int]]] = None
 
-    def __init__(
-        self,
-        *,
-        c_hash: Optional[str] = None,
-        c_list: Optional[List[List[int]]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            c_hash=c_hash,
-            c_list=c_list,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofProofAggregatedProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_proof_proofs_proof.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         non_revoc_proof: Indy non-revocation proof [Optional].
         primary_proof: Indy primary proof [Optional].
     """
 
     non_revoc_proof: Optional[IndyNonRevocProof] = None
     primary_proof: Optional[IndyPrimaryProof] = None
 
-    def __init__(
-        self,
-        *,
-        non_revoc_proof: Optional[IndyNonRevocProof] = None,
-        primary_proof: Optional[IndyPrimaryProof] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            non_revoc_proof=non_revoc_proof,
-            primary_proof=primary_proof,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofProofProofsProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_attr_spec.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,29 +26,12 @@
     """
 
     name: Optional[str] = None
     names: Optional[List[str]] = None
     non_revoked: Optional[IndyProofReqAttrSpecNonRevoked] = None
     restrictions: Optional[List[Dict[str, str]]] = None
 
-    def __init__(
-        self,
-        *,
-        name: Optional[str] = None,
-        names: Optional[List[str]] = None,
-        non_revoked: Optional[IndyProofReqAttrSpecNonRevoked] = None,
-        restrictions: Optional[List[Dict[str, str]]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            name=name,
-            names=names,
-            non_revoked=non_revoked,
-            restrictions=restrictions,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofReqAttrSpec.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_attr_spec_non_revoked.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         from_: Earliest time of interest in non-revocation interval [Optional].
         to: Latest time of interest in non-revocation interval [Optional].
     """
 
     from_: Optional[int] = Field(None, alias="from")
     to: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        from_: Optional[int] = None,
-        to: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            from_=from_,
-            to=to,
-            **kwargs,
-        )
-
     @validator("from_")
     def from__max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 18446744073709551615:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_pred_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,31 +28,12 @@
 
     name: str
     p_type: Literal["<", "<=", ">=", ">"]
     p_value: int
     non_revoked: Optional[IndyProofReqPredSpecNonRevoked] = None
     restrictions: Optional[List[Dict[str, str]]] = None
 
-    def __init__(
-        self,
-        *,
-        name: str = None,
-        p_type: Literal["<", "<=", ">=", ">"] = None,
-        p_value: int = None,
-        non_revoked: Optional[IndyProofReqPredSpecNonRevoked] = None,
-        restrictions: Optional[List[Dict[str, str]]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            name=name,
-            non_revoked=non_revoked,
-            p_type=p_type,
-            p_value=p_value,
-            restrictions=restrictions,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofReqPredSpec.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_request_non_revoked.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,40 +6,27 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyProofReqPredSpecNonRevoked(BaseModel):
+class IndyProofRequestNonRevoked(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofReqPredSpecNonRevoked - a model defined in OpenAPI
+    IndyProofRequestNonRevoked - a model defined in OpenAPI
         from_: Earliest time of interest in non-revocation interval [Optional].
         to: Latest time of interest in non-revocation interval [Optional].
     """
 
     from_: Optional[int] = Field(None, alias="from")
     to: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        from_: Optional[int] = None,
-        to: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            from_=from_,
-            to=to,
-            **kwargs,
-        )
-
     @validator("from_")
     def from__max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 18446744073709551615:
@@ -80,8 +67,8 @@
             raise ValueError(f"to must be greater than 0, currently {value}")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofReqPredSpecNonRevoked.update_forward_refs()
+IndyProofRequestNonRevoked.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/model_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,74 +4,67 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.indy_proof_req_attr_spec import IndyProofReqAttrSpec
-from aries_cloudcontroller.model.indy_proof_req_pred_spec import IndyProofReqPredSpec
-from aries_cloudcontroller.model.indy_proof_request_non_revoked import (
-    IndyProofRequestNonRevoked,
-)
 
 
-class IndyProofRequest(BaseModel):
+class ModelSchema(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofRequest - a model defined in OpenAPI
-        requested_attributes: Requested attribute specifications of proof request.
-        requested_predicates: Requested predicate specifications of proof request.
-        name: Proof request name [Optional].
-        non_revoked: The non_revoked of this IndyProofRequest [Optional].
-        nonce: Nonce [Optional].
-        version: Proof request version [Optional].
+    ModelSchema - a model defined in OpenAPI
+        attr_names: Schema attribute names [Optional].
+        id: Schema identifier [Optional].
+        name: Schema name [Optional].
+        seq_no: Schema sequence number [Optional].
+        ver: Node protocol version [Optional].
+        version: Schema version [Optional].
     """
 
-    requested_attributes: Dict[str, IndyProofReqAttrSpec]
-    requested_predicates: Dict[str, IndyProofReqPredSpec]
+    attr_names: Optional[List[str]] = Field(None, alias="attrNames")
+    id: Optional[str] = None
     name: Optional[str] = None
-    non_revoked: Optional[IndyProofRequestNonRevoked] = None
-    nonce: Optional[str] = None
+    seq_no: Optional[int] = Field(None, alias="seqNo")
+    ver: Optional[str] = None
     version: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        requested_attributes: Dict[str, IndyProofReqAttrSpec] = None,
-        requested_predicates: Dict[str, IndyProofReqPredSpec] = None,
-        name: Optional[str] = None,
-        non_revoked: Optional[IndyProofRequestNonRevoked] = None,
-        nonce: Optional[str] = None,
-        version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            name=name,
-            non_revoked=non_revoked,
-            nonce=nonce,
-            requested_attributes=requested_attributes,
-            requested_predicates=requested_predicates,
-            version=version,
-            **kwargs,
-        )
+    @validator("id")
+    def id_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+        if not re.match(pattern, value):
+            raise ValueError(f"Value of id does not match regex pattern ('{pattern}')")
+        return value
 
-    @validator("nonce")
-    def nonce_pattern(cls, value):
+    @validator("seq_no")
+    def seq_no_min(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[1-9][0-9]*$"
+        if value < 1:
+            raise ValueError(f"seq_no must be greater than 1, currently {value}")
+        return value
+
+    @validator("ver")
+    def ver_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[0-9.]+$"
         if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of nonce does not match regex pattern ('{pattern}')"
-            )
+            raise ValueError(f"Value of ver does not match regex pattern ('{pattern}')")
         return value
 
     @validator("version")
     def version_pattern(cls, value):
         # Property is optional
         if value is None:
             return
@@ -83,8 +76,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofRequest.update_forward_refs()
+ModelSchema.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_request_non_revoked.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_ld_proof.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,82 +6,59 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyProofRequestNonRevoked(BaseModel):
+class V20CredExRecordLDProof(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofRequestNonRevoked - a model defined in OpenAPI
-        from_: Earliest time of interest in non-revocation interval [Optional].
-        to: Latest time of interest in non-revocation interval [Optional].
+    V20CredExRecordLDProof - a model defined in OpenAPI
+        created_at: Time of record creation [Optional].
+        cred_ex_id: Corresponding v2.0 credential exchange record identifier [Optional].
+        cred_ex_ld_proof_id: Record identifier [Optional].
+        cred_id_stored: Credential identifier stored in wallet [Optional].
+        state: Current record state [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
-    from_: Optional[int] = Field(None, alias="from")
-    to: Optional[int] = None
+    created_at: Optional[str] = None
+    cred_ex_id: Optional[str] = None
+    cred_ex_ld_proof_id: Optional[str] = None
+    cred_id_stored: Optional[str] = None
+    state: Optional[str] = None
+    updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        from_: Optional[int] = None,
-        to: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            from_=from_,
-            to=to,
-            **kwargs,
-        )
-
-    @validator("from_")
-    def from__max(cls, value):
+    @validator("created_at")
+    def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value > 18446744073709551615:
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        if not re.match(pattern, value):
             raise ValueError(
-                f"from_ must be less than 18446744073709551615, currently {value}"
+                f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("from_")
-    def from__min(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        if value < 0:
-            raise ValueError(f"from_ must be greater than 0, currently {value}")
-        return value
-
-    @validator("to")
-    def to_max(cls, value):
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value > 18446744073709551615:
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        if not re.match(pattern, value):
             raise ValueError(
-                f"to must be less than 18446744073709551615, currently {value}"
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("to")
-    def to_min(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        if value < 0:
-            raise ValueError(f"to must be greater than 0, currently {value}")
-        return value
-
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofRequestNonRevoked.update_forward_refs()
+V20CredExRecordLDProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_predicate.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     IndyProofRequestedProofPredicate - a model defined in OpenAPI
         sub_proof_index: Sub-proof index [Optional].
     """
 
     sub_proof_index: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        sub_proof_index: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            sub_proof_index=sub_proof_index,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyProofRequestedProofPredicate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,29 +21,14 @@
         sub_proof_index: Sub-proof index [Optional].
     """
 
     encoded: Optional[str] = None
     raw: Optional[str] = None
     sub_proof_index: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        encoded: Optional[str] = None,
-        raw: Optional[str] = None,
-        sub_proof_index: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            encoded=encoded,
-            raw=raw,
-            sub_proof_index=sub_proof_index,
-            **kwargs,
-        )
-
     @validator("encoded")
     def encoded_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^-?[0-9]*$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_proposal_by_format.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,41 +4,29 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.raw_encoded import RawEncoded
+from aries_cloudcontroller.model.dif_proof_proposal import DIFProofProposal
+from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
 
 
-class IndyProofRequestedProofRevealedAttrGroup(BaseModel):
+class V20PresProposalByFormat(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyProofRequestedProofRevealedAttrGroup - a model defined in OpenAPI
-        sub_proof_index: Sub-proof index [Optional].
-        values: Indy proof requested proof revealed attr groups group value [Optional].
+    V20PresProposalByFormat - a model defined in OpenAPI
+        dif: Presentation proposal for DIF [Optional].
+        indy: Presentation proposal for indy [Optional].
     """
 
-    sub_proof_index: Optional[int] = None
-    values: Optional[Dict[str, RawEncoded]] = None
-
-    def __init__(
-        self,
-        *,
-        sub_proof_index: Optional[int] = None,
-        values: Optional[Dict[str, RawEncoded]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            sub_proof_index=sub_proof_index,
-            values=values,
-            **kwargs,
-        )
+    dif: Optional[DIFProofProposal] = None
+    indy: Optional[IndyProofRequest] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyProofRequestedProofRevealedAttrGroup.update_forward_refs()
+V20PresProposalByFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_requested_creds_requested_attr.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         cred_id: Wallet credential identifier (typically but not necessarily a UUID).
         revealed: Whether to reveal attribute in proof (default true) [Optional].
     """
 
     cred_id: str
     revealed: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        cred_id: str = None,
-        revealed: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_id=cred_id,
-            revealed=revealed,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyRequestedCredsRequestedAttr.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_requested_creds_requested_pred.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_req_pred_spec_non_revoked.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,60 +6,69 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IndyRequestedCredsRequestedPred(BaseModel):
+class IndyProofReqPredSpecNonRevoked(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyRequestedCredsRequestedPred - a model defined in OpenAPI
-        cred_id: Wallet credential identifier (typically but not necessarily a UUID).
-        timestamp: Epoch timestamp of interest for non-revocation proof [Optional].
+    IndyProofReqPredSpecNonRevoked - a model defined in OpenAPI
+        from_: Earliest time of interest in non-revocation interval [Optional].
+        to: Latest time of interest in non-revocation interval [Optional].
     """
 
-    cred_id: str
-    timestamp: Optional[int] = None
+    from_: Optional[int] = Field(None, alias="from")
+    to: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        cred_id: str = None,
-        timestamp: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_id=cred_id,
-            timestamp=timestamp,
-            **kwargs,
-        )
+    @validator("from_")
+    def from__max(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value > 18446744073709551615:
+            raise ValueError(
+                f"from_ must be less than 18446744073709551615, currently {value}"
+            )
+        return value
+
+    @validator("from_")
+    def from__min(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        if value < 0:
+            raise ValueError(f"from_ must be greater than 0, currently {value}")
+        return value
 
-    @validator("timestamp")
-    def timestamp_max(cls, value):
+    @validator("to")
+    def to_max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 18446744073709551615:
             raise ValueError(
-                f"timestamp must be less than 18446744073709551615, currently {value}"
+                f"to must be less than 18446744073709551615, currently {value}"
             )
         return value
 
-    @validator("timestamp")
-    def timestamp_min(cls, value):
+    @validator("to")
+    def to_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
-            raise ValueError(f"timestamp must be greater than 0, currently {value}")
+            raise ValueError(f"to must be greater than 0, currently {value}")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyRequestedCredsRequestedPred.update_forward_refs()
+IndyProofReqPredSpecNonRevoked.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,35 +28,14 @@
     cred_def_id: Optional[str] = Field(None, alias="credDefId")
     id: Optional[str] = None
     revoc_def_type: Optional[Literal["CL_ACCUM"]] = Field(None, alias="revocDefType")
     tag: Optional[str] = None
     value: Optional[IndyRevRegDefValue] = None
     ver: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        cred_def_id: Optional[str] = None,
-        id: Optional[str] = None,
-        revoc_def_type: Optional[Literal["CL_ACCUM"]] = None,
-        tag: Optional[str] = None,
-        value: Optional[IndyRevRegDefValue] = None,
-        ver: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            id=id,
-            revoc_def_type=revoc_def_type,
-            tag=tag,
-            value=value,
-            ver=ver,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,35 +32,14 @@
     max_cred_num: Optional[int] = Field(None, alias="maxCredNum")
     public_keys: Optional[IndyRevRegDefValuePublicKeys] = Field(
         None, alias="publicKeys"
     )
     tails_hash: Optional[str] = Field(None, alias="tailsHash")
     tails_location: Optional[str] = Field(None, alias="tailsLocation")
 
-    def __init__(
-        self,
-        *,
-        issuance_type: Optional[
-            Literal["ISSUANCE_ON_DEMAND", "ISSUANCE_BY_DEFAULT"]
-        ] = None,
-        max_cred_num: Optional[int] = None,
-        public_keys: Optional[IndyRevRegDefValuePublicKeys] = None,
-        tails_hash: Optional[str] = None,
-        tails_location: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            issuance_type=issuance_type,
-            max_cred_num=max_cred_num,
-            public_keys=public_keys,
-            tails_hash=tails_hash,
-            tails_location=tails_location,
-            **kwargs,
-        )
-
     @validator("max_cred_num")
     def max_cred_num_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 1:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,23 +22,12 @@
         accum_key: The accum_key of this IndyRevRegDefValuePublicKeys [Optional].
     """
 
     accum_key: Optional[IndyRevRegDefValuePublicKeysAccumKey] = Field(
         None, alias="accumKey"
     )
 
-    def __init__(
-        self,
-        *,
-        accum_key: Optional[IndyRevRegDefValuePublicKeysAccumKey] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            accum_key=accum_key,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyRevRegDefValuePublicKeys.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_def_value_public_keys_accum_key.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     IndyRevRegDefValuePublicKeysAccumKey - a model defined in OpenAPI
         z: Value for z [Optional].
     """
 
     z: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        z: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            z=z,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 IndyRevRegDefValuePublicKeysAccumKey.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_entry.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_rev_reg_entry.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,27 +20,14 @@
         value: Revocation registry entry value [Optional].
         ver: Version of revocation registry entry [Optional].
     """
 
     value: Optional[IndyRevRegEntryValue] = None
     ver: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        value: Optional[IndyRevRegEntryValue] = None,
-        ver: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            value=value,
-            ver=ver,
-            **kwargs,
-        )
-
     @validator("ver")
     def ver_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9.]+$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/indy_rev_reg_entry_value.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_option.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,44 +4,34 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.menu_form import MenuForm
 
 
-class IndyRevRegEntryValue(BaseModel):
+class MenuOption(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IndyRevRegEntryValue - a model defined in OpenAPI
-        accum: Accumulator value [Optional].
-        prev_accum: Previous accumulator value [Optional].
-        revoked: Revoked credential revocation identifiers [Optional].
+    MenuOption - a model defined in OpenAPI
+        name: Menu option name (unique identifier).
+        title: Menu option title.
+        description: Additional descriptive text for menu option [Optional].
+        disabled: Whether to show option as disabled [Optional].
+        form: The form of this MenuOption [Optional].
     """
 
-    accum: Optional[str] = None
-    prev_accum: Optional[str] = Field(None, alias="prevAccum")
-    revoked: Optional[List[int]] = None
-
-    def __init__(
-        self,
-        *,
-        accum: Optional[str] = None,
-        prev_accum: Optional[str] = None,
-        revoked: Optional[List[int]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            accum=accum,
-            prev_accum=prev_accum,
-            revoked=revoked,
-            **kwargs,
-        )
+    name: str
+    title: str
+    description: Optional[str] = None
+    disabled: Optional[bool] = None
+    form: Optional[MenuForm] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-IndyRevRegEntryValue.update_forward_refs()
+MenuOption.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_create_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/connection_invitation.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,82 +4,50 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attachment_def import AttachmentDef
 
 
-class InvitationCreateRequest(BaseModel):
+class ConnectionInvitation(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    InvitationCreateRequest - a model defined in OpenAPI
-        accept: List of mime type in order of preference that should be use in responding to the message [Optional].
-        alias: Alias for connection [Optional].
-        attachments: Optional invitation attachments [Optional].
-        handshake_protocols: The handshake_protocols of this InvitationCreateRequest [Optional].
-        mediation_id: Identifier for active mediation record to be used [Optional].
-        metadata: Optional metadata to attach to the connection created with the invitation [Optional].
-        my_label: Label for connection invitation [Optional].
-        protocol_version: OOB protocol version [Optional].
-        use_public_did: Whether to use public DID in invitation [Optional].
+    ConnectionInvitation - a model defined in OpenAPI
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        did: DID for connection invitation [Optional].
+        image_url: Optional image URL for connection invitation [Optional].
+        label: Optional label for connection invitation [Optional].
+        recipient_keys: List of recipient keys [Optional].
+        routing_keys: List of routing keys [Optional].
+        service_endpoint: Service endpoint at which to reach this agent [Optional].
     """
 
-    accept: Optional[List[str]] = None
-    alias: Optional[str] = None
-    attachments: Optional[List[AttachmentDef]] = None
-    handshake_protocols: Optional[List[str]] = None
-    mediation_id: Optional[str] = None
-    metadata: Optional[Dict[str, Any]] = None
-    my_label: Optional[str] = None
-    protocol_version: Optional[str] = None
-    use_public_did: Optional[bool] = None
-
-    def __init__(
-        self,
-        *,
-        accept: Optional[List[str]] = None,
-        alias: Optional[str] = None,
-        attachments: Optional[List[AttachmentDef]] = None,
-        handshake_protocols: Optional[List[str]] = None,
-        mediation_id: Optional[str] = None,
-        metadata: Optional[Dict[str, Any]] = None,
-        my_label: Optional[str] = None,
-        protocol_version: Optional[str] = None,
-        use_public_did: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            accept=accept,
-            alias=alias,
-            attachments=attachments,
-            handshake_protocols=handshake_protocols,
-            mediation_id=mediation_id,
-            metadata=metadata,
-            my_label=my_label,
-            protocol_version=protocol_version,
-            use_public_did=use_public_did,
-            **kwargs,
-        )
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    did: Optional[str] = None
+    image_url: Optional[str] = Field(None, alias="imageUrl")
+    label: Optional[str] = None
+    recipient_keys: Optional[List[str]] = Field(None, alias="recipientKeys")
+    routing_keys: Optional[List[str]] = Field(None, alias="routingKeys")
+    service_endpoint: Optional[str] = Field(None, alias="serviceEndpoint")
 
-    @validator("mediation_id")
-    def mediation_id_pattern(cls, value):
+    @validator("did")
+    def did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-4[a-fA-F0-9]{3}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of mediation_id does not match regex pattern ('{pattern}')"
-            )
+            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-InvitationCreateRequest.update_forward_refs()
+ConnectionInvitation.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_record.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,71 +4,55 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.invitation_message import InvitationMessage
 
 
-class InvitationRecord(BaseModel):
+class TransactionRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    InvitationRecord - a model defined in OpenAPI
+    TransactionRecord - a model defined in OpenAPI
+        type: Transaction type [Optional].
+        connection_id: The connection identifier for thie particular transaction record [Optional].
         created_at: Time of record creation [Optional].
-        invi_msg_id: Invitation message identifier [Optional].
-        invitation: Out of band invitation message [Optional].
-        invitation_id: Invitation record identifier [Optional].
-        invitation_url: Invitation message URL [Optional].
-        oob_id: Out of band record identifier [Optional].
-        state: Out of band message exchange state [Optional].
+        endorser_write_txn: If True, Endorser will write the transaction after endorsing it [Optional].
+        formats: The formats of this TransactionRecord [Optional].
+        messages_attach: The messages_attach of this TransactionRecord [Optional].
+        meta_data: The meta_data of this TransactionRecord [Optional].
+        signature_request: The signature_request of this TransactionRecord [Optional].
+        signature_response: The signature_response of this TransactionRecord [Optional].
+        state: Current record state [Optional].
+        thread_id: Thread Identifier [Optional].
+        timing: The timing of this TransactionRecord [Optional].
         trace: Record trace information, based on agent configuration [Optional].
+        transaction_id: Transaction identifier [Optional].
         updated_at: Time of last record update [Optional].
     """
 
+    type: Optional[str] = Field(None, alias="_type")
+    connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    invi_msg_id: Optional[str] = None
-    invitation: Optional[InvitationMessage] = None
-    invitation_id: Optional[str] = None
-    invitation_url: Optional[str] = None
-    oob_id: Optional[str] = None
+    endorser_write_txn: Optional[bool] = None
+    formats: Optional[List[Dict[str, str]]] = None
+    messages_attach: Optional[List[Dict]] = None
+    meta_data: Optional[Dict[str, Any]] = None
+    signature_request: Optional[List[Dict]] = None
+    signature_response: Optional[List[Dict]] = None
     state: Optional[str] = None
+    thread_id: Optional[str] = None
+    timing: Optional[Dict[str, Any]] = None
     trace: Optional[bool] = None
+    transaction_id: Optional[str] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        created_at: Optional[str] = None,
-        invi_msg_id: Optional[str] = None,
-        invitation: Optional[InvitationMessage] = None,
-        invitation_id: Optional[str] = None,
-        invitation_url: Optional[str] = None,
-        oob_id: Optional[str] = None,
-        state: Optional[str] = None,
-        trace: Optional[bool] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            invi_msg_id=invi_msg_id,
-            invitation=invitation,
-            invitation_id=invitation_id,
-            invitation_url=invitation_url,
-            oob_id=oob_id,
-            state=state,
-            trace=trace,
-            updated_at=updated_at,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
@@ -91,8 +75,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-InvitationRecord.update_forward_refs()
+TransactionRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/invitation_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,27 +22,12 @@
         invitation_url: Invitation URL [Optional].
     """
 
     connection_id: Optional[str] = None
     invitation: Optional[ConnectionInvitation] = None
     invitation_url: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: Optional[str] = None,
-        invitation: Optional[ConnectionInvitation] = None,
-        invitation_url: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            connection_id=connection_id,
-            invitation=invitation,
-            invitation_url=invitation_url,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 InvitationResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/issuer_cred_rev_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/conn_record.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,117 +6,114 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class IssuerCredRevRecord(BaseModel):
+class ConnRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IssuerCredRevRecord - a model defined in OpenAPI
+    ConnRecord - a model defined in OpenAPI
+        accept: Connection acceptance: manual or auto [Optional].
+        alias: Optional alias to apply to connection for later use [Optional].
+        connection_id: Connection identifier [Optional].
+        connection_protocol: Connection protocol used [Optional].
         created_at: Time of record creation [Optional].
-        cred_def_id: Credential definition identifier [Optional].
-        cred_ex_id: Credential exchange record identifier at credential issue [Optional].
-        cred_ex_version: Credential exchange version [Optional].
-        cred_rev_id: Credential revocation identifier [Optional].
-        record_id: Issuer credential revocation record identifier [Optional].
-        rev_reg_id: Revocation registry identifier [Optional].
-        state: Issue credential revocation record state [Optional].
+        error_msg: Error message [Optional].
+        inbound_connection_id: Inbound routing connection id to use [Optional].
+        invitation_key: Public key for connection [Optional].
+        invitation_mode: Invitation mode [Optional].
+        invitation_msg_id: ID of out-of-band invitation message [Optional].
+        my_did: Our DID for connection [Optional].
+        request_id: Connection request identifier [Optional].
+        rfc23_state: State per RFC 23 [Optional].
+        routing_state: Routing state of connection [Optional].
+        state: Current record state [Optional].
+        their_did: Their DID for connection [Optional].
+        their_label: Their label for connection [Optional].
+        their_public_did: Other agent&#39;s public DID for connection [Optional].
+        their_role: Their role in the connection protocol [Optional].
         updated_at: Time of last record update [Optional].
     """
 
+    accept: Optional[Literal["manual", "auto"]] = None
+    alias: Optional[str] = None
+    connection_id: Optional[str] = None
+    connection_protocol: Optional[Literal["connections/1.0", "didexchange/1.0"]] = None
     created_at: Optional[str] = None
-    cred_def_id: Optional[str] = None
-    cred_ex_id: Optional[str] = None
-    cred_ex_version: Optional[str] = None
-    cred_rev_id: Optional[str] = None
-    record_id: Optional[str] = None
-    rev_reg_id: Optional[str] = None
+    error_msg: Optional[str] = None
+    inbound_connection_id: Optional[str] = None
+    invitation_key: Optional[str] = None
+    invitation_mode: Optional[Literal["once", "multi", "static"]] = None
+    invitation_msg_id: Optional[str] = None
+    my_did: Optional[str] = None
+    request_id: Optional[str] = None
+    rfc23_state: Optional[str] = None
+    routing_state: Optional[Literal["none", "request", "active", "error"]] = None
     state: Optional[str] = None
+    their_did: Optional[str] = None
+    their_label: Optional[str] = None
+    their_public_did: Optional[str] = None
+    their_role: Optional[Literal["invitee", "requester", "inviter", "responder"]] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        created_at: Optional[str] = None,
-        cred_def_id: Optional[str] = None,
-        cred_ex_id: Optional[str] = None,
-        cred_ex_version: Optional[str] = None,
-        cred_rev_id: Optional[str] = None,
-        record_id: Optional[str] = None,
-        rev_reg_id: Optional[str] = None,
-        state: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            cred_def_id=cred_def_id,
-            cred_ex_id=cred_ex_id,
-            cred_ex_version=cred_ex_version,
-            cred_rev_id=cred_rev_id,
-            record_id=record_id,
-            rev_reg_id=rev_reg_id,
-            state=state,
-            updated_at=updated_at,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("cred_def_id")
-    def cred_def_id_pattern(cls, value):
+    @validator("invitation_key")
+    def invitation_key_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
+        pattern = (
+            r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
+        )
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
+                f"Value of invitation_key does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("cred_rev_id")
-    def cred_rev_id_pattern(cls, value):
+    @validator("my_did")
+    def my_did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[1-9][0-9]*$"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of cred_rev_id does not match regex pattern ('{pattern}')"
+                f"Value of my_did does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("rev_reg_id")
-    def rev_reg_id_pattern(cls, value):
+    @validator("their_did")
+    def their_did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of rev_reg_id does not match regex pattern ('{pattern}')"
+                f"Value of their_did does not match regex pattern ('{pattern}')"
             )
         return value
 
     @validator("updated_at")
     def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
@@ -129,8 +126,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IssuerCredRevRecord.update_forward_refs()
+ConnRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/issuer_rev_reg_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_exchange.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,168 +4,119 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.indy_rev_reg_def import IndyRevRegDef
-from aries_cloudcontroller.model.indy_rev_reg_entry import IndyRevRegEntry
+from aries_cloudcontroller.model.credential_offer import CredentialOffer
+from aries_cloudcontroller.model.credential_proposal import CredentialProposal
+from aries_cloudcontroller.model.indy_cred_abstract import IndyCredAbstract
+from aries_cloudcontroller.model.indy_cred_info import IndyCredInfo
+from aries_cloudcontroller.model.indy_cred_request import IndyCredRequest
+from aries_cloudcontroller.model.indy_credential import IndyCredential
 
 
-class IssuerRevRegRecord(BaseModel):
+class V10CredentialExchange(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    IssuerRevRegRecord - a model defined in OpenAPI
+    V10CredentialExchange - a model defined in OpenAPI
+        auto_issue: Issuer choice to issue to request in this credential exchange [Optional].
+        auto_offer: Holder choice to accept offer in this credential exchange [Optional].
+        auto_remove: Issuer choice to remove this credential exchange record when complete [Optional].
+        connection_id: Connection identifier [Optional].
         created_at: Time of record creation [Optional].
-        cred_def_id: Credential definition identifier [Optional].
+        credential: Credential as stored [Optional].
+        credential_definition_id: Credential definition identifier [Optional].
+        credential_exchange_id: Credential exchange identifier [Optional].
+        credential_id: Credential identifier [Optional].
+        credential_offer: (Indy) credential offer [Optional].
+        credential_offer_dict: Credential offer message [Optional].
+        credential_proposal_dict: Credential proposal message [Optional].
+        credential_request: (Indy) credential request [Optional].
+        credential_request_metadata: (Indy) credential request metadata [Optional].
         error_msg: Error message [Optional].
-        issuer_did: Issuer DID [Optional].
-        max_cred_num: Maximum number of credentials for revocation registry [Optional].
-        pending_pub: Credential revocation identifier for credential revoked and pending publication to ledger [Optional].
-        record_id: Issuer revocation registry record identifier [Optional].
-        revoc_def_type: Revocation registry type (specify CL_ACCUM) [Optional].
-        revoc_reg_def: Revocation registry definition [Optional].
-        revoc_reg_entry: Revocation registry entry [Optional].
+        initiator: Issue-credential exchange initiator: self or external [Optional].
+        parent_thread_id: Parent thread identifier [Optional].
+        raw_credential: Credential as received, prior to storage in holder wallet [Optional].
         revoc_reg_id: Revocation registry identifier [Optional].
-        state: Issue revocation registry record state [Optional].
-        tag: Tag within issuer revocation registry identifier [Optional].
-        tails_hash: Tails hash [Optional].
-        tails_local_path: Local path to tails file [Optional].
-        tails_public_uri: Public URI for tails file [Optional].
+        revocation_id: Credential identifier within revocation registry [Optional].
+        role: Issue-credential exchange role: holder or issuer [Optional].
+        schema_id: Schema identifier [Optional].
+        state: Issue-credential exchange state [Optional].
+        thread_id: Thread identifier [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
     """
 
+    auto_issue: Optional[bool] = None
+    auto_offer: Optional[bool] = None
+    auto_remove: Optional[bool] = None
+    connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    cred_def_id: Optional[str] = None
+    credential: Optional[IndyCredInfo] = None
+    credential_definition_id: Optional[str] = None
+    credential_exchange_id: Optional[str] = None
+    credential_id: Optional[str] = None
+    credential_offer: Optional[IndyCredAbstract] = None
+    credential_offer_dict: Optional[CredentialOffer] = None
+    credential_proposal_dict: Optional[CredentialProposal] = None
+    credential_request: Optional[IndyCredRequest] = None
+    credential_request_metadata: Optional[Dict[str, Any]] = None
     error_msg: Optional[str] = None
-    issuer_did: Optional[str] = None
-    max_cred_num: Optional[int] = None
-    pending_pub: Optional[List[str]] = None
-    record_id: Optional[str] = None
-    revoc_def_type: Optional[Literal["CL_ACCUM"]] = None
-    revoc_reg_def: Optional[IndyRevRegDef] = None
-    revoc_reg_entry: Optional[IndyRevRegEntry] = None
+    initiator: Optional[Literal["self", "external"]] = None
+    parent_thread_id: Optional[str] = None
+    raw_credential: Optional[IndyCredential] = None
     revoc_reg_id: Optional[str] = None
+    revocation_id: Optional[str] = None
+    role: Optional[Literal["holder", "issuer"]] = None
+    schema_id: Optional[str] = None
     state: Optional[str] = None
-    tag: Optional[str] = None
-    tails_hash: Optional[str] = None
-    tails_local_path: Optional[str] = None
-    tails_public_uri: Optional[str] = None
+    thread_id: Optional[str] = None
+    trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        created_at: Optional[str] = None,
-        cred_def_id: Optional[str] = None,
-        error_msg: Optional[str] = None,
-        issuer_did: Optional[str] = None,
-        max_cred_num: Optional[int] = None,
-        pending_pub: Optional[List[str]] = None,
-        record_id: Optional[str] = None,
-        revoc_def_type: Optional[Literal["CL_ACCUM"]] = None,
-        revoc_reg_def: Optional[IndyRevRegDef] = None,
-        revoc_reg_entry: Optional[IndyRevRegEntry] = None,
-        revoc_reg_id: Optional[str] = None,
-        state: Optional[str] = None,
-        tag: Optional[str] = None,
-        tails_hash: Optional[str] = None,
-        tails_local_path: Optional[str] = None,
-        tails_public_uri: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            cred_def_id=cred_def_id,
-            error_msg=error_msg,
-            issuer_did=issuer_did,
-            max_cred_num=max_cred_num,
-            pending_pub=pending_pub,
-            record_id=record_id,
-            revoc_def_type=revoc_def_type,
-            revoc_reg_def=revoc_reg_def,
-            revoc_reg_entry=revoc_reg_entry,
-            revoc_reg_id=revoc_reg_id,
-            state=state,
-            tag=tag,
-            tails_hash=tails_hash,
-            tails_local_path=tails_local_path,
-            tails_public_uri=tails_public_uri,
-            updated_at=updated_at,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("cred_def_id")
-    def cred_def_id_pattern(cls, value):
+    @validator("credential_definition_id")
+    def credential_definition_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
-            )
-        return value
-
-    @validator("issuer_did")
-    def issuer_did_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
-        if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of issuer_did does not match regex pattern ('{pattern}')"
-            )
-        return value
-
-    @validator("revoc_reg_id")
-    def revoc_reg_id_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
-        if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of revoc_reg_id does not match regex pattern ('{pattern}')"
+                f"Value of credential_definition_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("tails_hash")
-    def tails_hash_pattern(cls, value):
+    @validator("schema_id")
+    def schema_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = (
-            r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
-        )
+        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of tails_hash does not match regex pattern ('{pattern}')"
+                f"Value of schema_id does not match regex pattern ('{pattern}')"
             )
         return value
 
     @validator("updated_at")
     def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
@@ -178,8 +129,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-IssuerRevRegRecord.update_forward_refs()
+V10CredentialExchange.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/wallet_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.route_record import RouteRecord
+from aries_cloudcontroller.model.wallet_record import WalletRecord
 
 
-class Keylist(BaseModel):
+class WalletList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Keylist - a model defined in OpenAPI
-        results: List of keylist records [Optional].
+    WalletList - a model defined in OpenAPI
+        results: List of wallet records [Optional].
     """
 
-    results: Optional[List[RouteRecord]] = None
-
-    def __init__(
-        self,
-        *,
-        results: Optional[List[RouteRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
+    results: Optional[List[WalletRecord]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Keylist.update_forward_refs()
+WalletList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,29 +24,12 @@
     """
 
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     filter: Optional[Dict[str, Any]] = None
     paginate: Optional[KeylistQueryPaginate] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        filter: Optional[Dict[str, Any]] = None,
-        paginate: Optional[KeylistQueryPaginate] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            filter=filter,
-            paginate=paginate,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 KeylistQuery.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query_filter_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,36 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.keylist_update_rule import KeylistUpdateRule
 
 
-class KeylistQueryFilterRequest(BaseModel):
+class KeylistUpdateRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    KeylistQueryFilterRequest - a model defined in OpenAPI
-        filter: Filter for keylist query [Optional].
+    KeylistUpdateRequest - a model defined in OpenAPI
+        updates: The updates of this KeylistUpdateRequest [Optional].
     """
 
-    filter: Optional[Dict[str, Any]] = None
-
-    def __init__(
-        self,
-        *,
-        filter: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            filter=filter,
-            **kwargs,
-        )
+    updates: Optional[List[KeylistUpdateRule]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-KeylistQueryFilterRequest.update_forward_refs()
+KeylistUpdateRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_query_paginate.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ping_request_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,38 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class KeylistQueryPaginate(BaseModel):
+class PingRequestResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    KeylistQueryPaginate - a model defined in OpenAPI
-        limit: Limit for keylist query [Optional].
-        offset: Offset value for query [Optional].
+    PingRequestResponse - a model defined in OpenAPI
+        thread_id: Thread ID of the ping message [Optional].
     """
 
-    limit: Optional[int] = None
-    offset: Optional[int] = None
-
-    def __init__(
-        self,
-        *,
-        limit: Optional[int] = None,
-        offset: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            limit=limit,
-            offset=offset,
-            **kwargs,
-        )
+    thread_id: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-KeylistQueryPaginate.update_forward_refs()
+PingRequestResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,27 +22,12 @@
         updates: List of update rules [Optional].
     """
 
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     updates: Optional[List[KeylistUpdateRule]] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        updates: Optional[List[KeylistUpdateRule]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            updates=updates,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 KeylistUpdate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schemas_input_descriptor_filter.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,37 +4,28 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.keylist_update_rule import KeylistUpdateRule
+from aries_cloudcontroller.model.schema_input_descriptor import SchemaInputDescriptor
 
 
-class KeylistUpdateRequest(BaseModel):
+class SchemasInputDescriptorFilter(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    KeylistUpdateRequest - a model defined in OpenAPI
-        updates: The updates of this KeylistUpdateRequest [Optional].
+    SchemasInputDescriptorFilter - a model defined in OpenAPI
+        oneof_filter: oneOf [Optional].
+        uri_groups: The uri_groups of this SchemasInputDescriptorFilter [Optional].
     """
 
-    updates: Optional[List[KeylistUpdateRule]] = None
-
-    def __init__(
-        self,
-        *,
-        updates: Optional[List[KeylistUpdateRule]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            updates=updates,
-            **kwargs,
-        )
+    oneof_filter: Optional[bool] = None
+    uri_groups: Optional[List[List[SchemaInputDescriptor]]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-KeylistUpdateRequest.update_forward_refs()
+SchemasInputDescriptorFilter.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/keylist_update_rule.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_update_rule.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         action: Action for specific key.
         recipient_key: Key to remove or add.
     """
 
     action: Literal["add", "remove"]
     recipient_key: str
 
-    def __init__(
-        self,
-        *,
-        action: Literal["add", "remove"] = None,
-        recipient_key: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            action=action,
-            recipient_key=recipient_key,
-            **kwargs,
-        )
-
     @validator("recipient_key")
     def recipient_key_pattern(cls, value):
         pattern = r"^did:key:z[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]+$|^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of recipient_key does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ld_proof_vc_detail.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ld_proof_vc_detail.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,25 +23,12 @@
         credential: Detail of the JSON-LD Credential to be issued.
         options: Options for specifying how the linked data proof is created..
     """
 
     credential: Credential
     options: LDProofVCDetailOptions
 
-    def __init__(
-        self,
-        *,
-        credential: Credential = None,
-        options: LDProofVCDetailOptions = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential=credential,
-            options=options,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 LDProofVCDetail.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ld_proof_vc_detail_options.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ld_proof_vc_detail_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,35 +32,14 @@
     created: Optional[str] = None
     credential_status: Optional[CredentialStatusOptions] = Field(
         None, alias="credentialStatus"
     )
     domain: Optional[str] = None
     proof_purpose: Optional[str] = Field(None, alias="proofPurpose")
 
-    def __init__(
-        self,
-        *,
-        proof_type: str = None,
-        challenge: Optional[str] = None,
-        created: Optional[str] = None,
-        credential_status: Optional[CredentialStatusOptions] = None,
-        domain: Optional[str] = None,
-        proof_purpose: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            challenge=challenge,
-            created=created,
-            credential_status=credential_status,
-            domain=domain,
-            proof_purpose=proof_purpose,
-            proof_type=proof_type,
-            **kwargs,
-        )
-
     @validator("created")
     def created_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ledger_config_instance.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ledger_config_instance.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,31 +25,12 @@
 
     genesis_file: Optional[str] = None
     genesis_transactions: Optional[str] = None
     genesis_url: Optional[str] = None
     id: Optional[str] = None
     is_production: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        genesis_file: Optional[str] = None,
-        genesis_transactions: Optional[str] = None,
-        genesis_url: Optional[str] = None,
-        id: Optional[str] = None,
-        is_production: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            genesis_file=genesis_file,
-            genesis_transactions=genesis_transactions,
-            genesis_url=genesis_url,
-            id=id,
-            is_production=is_production,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 LedgerConfigInstance.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/linked_data_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,97 +6,67 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class LinkedDataProof(BaseModel):
+class MediationRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    LinkedDataProof - a model defined in OpenAPI
-        created: The string value of an ISO8601 combined date and time string generated by the Signature Algorithm.
-        proof_purpose: Proof purpose.
-        type: Identifies the digital signature suite that was used to create the signature.
-        verification_method: Information used for proof verification.
-        challenge: Associates a challenge with a proof, for use with a proofPurpose such as authentication [Optional].
-        domain: A string value specifying the restricted domain of the signature. [Optional].
-        jws: Associates a Detached Json Web Signature with a proof [Optional].
-        nonce: The nonce [Optional].
-        proof_value: The proof value of a proof [Optional].
+    MediationRecord - a model defined in OpenAPI
+        connection_id: The connection_id of this MediationRecord.
+        role: The role of this MediationRecord.
+        created_at: Time of record creation [Optional].
+        endpoint: The endpoint of this MediationRecord [Optional].
+        mediation_id: The mediation_id of this MediationRecord [Optional].
+        mediator_terms: The mediator_terms of this MediationRecord [Optional].
+        recipient_terms: The recipient_terms of this MediationRecord [Optional].
+        routing_keys: The routing_keys of this MediationRecord [Optional].
+        state: Current record state [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
-    created: str
-    proof_purpose: str = Field(..., alias="proofPurpose")
-    type: str
-    verification_method: str = Field(..., alias="verificationMethod")
-    challenge: Optional[str] = None
-    domain: Optional[str] = None
-    jws: Optional[str] = None
-    nonce: Optional[str] = None
-    proof_value: Optional[str] = Field(None, alias="proofValue")
-
-    def __init__(
-        self,
-        *,
-        created: str = None,
-        proof_purpose: str = None,
-        type: str = None,
-        verification_method: str = None,
-        challenge: Optional[str] = None,
-        domain: Optional[str] = None,
-        jws: Optional[str] = None,
-        nonce: Optional[str] = None,
-        proof_value: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            challenge=challenge,
-            created=created,
-            domain=domain,
-            jws=jws,
-            nonce=nonce,
-            proof_purpose=proof_purpose,
-            proof_value=proof_value,
-            type=type,
-            verification_method=verification_method,
-            **kwargs,
-        )
+    connection_id: str
+    role: str
+    created_at: Optional[str] = None
+    endpoint: Optional[str] = None
+    mediation_id: Optional[str] = None
+    mediator_terms: Optional[List[str]] = None
+    recipient_terms: Optional[List[str]] = None
+    routing_keys: Optional[List[str]] = None
+    state: Optional[str] = None
+    updated_at: Optional[str] = None
+
+    @validator("created_at")
+    def created_at_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
 
-    @validator("created")
-    def created_pattern(cls, value):
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of created does not match regex pattern ('{pattern}')"
+                f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("domain")
-    def domain_pattern(cls, value):
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"\w+:(\\/?\\/?)[^\s]+"
-        if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of domain does not match regex pattern ('{pattern}')"
-            )
-        return value
-
-    @validator("verification_method")
-    def verification_method_pattern(cls, value):
-        pattern = r"\w+:(\\/?\\/?)[^\s]+"
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of verification_method does not match regex pattern ('{pattern}')"
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-LinkedDataProof.update_forward_refs()
+MediationRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_create_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_create_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         mediator_terms: List of mediator rules for recipient [Optional].
         recipient_terms: List of recipient rules for mediation [Optional].
     """
 
     mediator_terms: Optional[List[str]] = None
     recipient_terms: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        mediator_terms: Optional[List[str]] = None,
-        recipient_terms: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mediator_terms=mediator_terms,
-            recipient_terms=recipient_terms,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 MediationCreateRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_deny.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/receive_invitation_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,46 +6,48 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class MediationDeny(BaseModel):
+class ReceiveInvitationRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    MediationDeny - a model defined in OpenAPI
+    ReceiveInvitationRequest - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
-        mediator_terms: The mediator_terms of this MediationDeny [Optional].
-        recipient_terms: The recipient_terms of this MediationDeny [Optional].
+        did: DID for connection invitation [Optional].
+        image_url: Optional image URL for connection invitation [Optional].
+        label: Optional label for connection invitation [Optional].
+        recipient_keys: List of recipient keys [Optional].
+        routing_keys: List of routing keys [Optional].
+        service_endpoint: Service endpoint at which to reach this agent [Optional].
     """
 
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
-    mediator_terms: Optional[List[str]] = None
-    recipient_terms: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        mediator_terms: Optional[List[str]] = None,
-        recipient_terms: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            mediator_terms=mediator_terms,
-            recipient_terms=recipient_terms,
-            **kwargs,
-        )
+    did: Optional[str] = None
+    image_url: Optional[str] = Field(None, alias="imageUrl")
+    label: Optional[str] = None
+    recipient_keys: Optional[List[str]] = Field(None, alias="recipientKeys")
+    routing_keys: Optional[List[str]] = Field(None, alias="routingKeys")
+    service_endpoint: Optional[str] = Field(None, alias="serviceEndpoint")
+
+    @validator("did")
+    def did_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        if not re.match(pattern, value):
+            raise ValueError(f"Value of did does not match regex pattern ('{pattern}')")
+        return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-MediationDeny.update_forward_refs()
+ReceiveInvitationRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_grant.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_grant.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,29 +23,12 @@
     """
 
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     endpoint: Optional[str] = None
     routing_keys: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        endpoint: Optional[str] = None,
-        routing_keys: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            endpoint=endpoint,
-            routing_keys=routing_keys,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 MediationGrant.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_id_match_info.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_id_match_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     MediationIdMatchInfo - a model defined in OpenAPI
         mediation_id: Mediation record identifier [Optional].
     """
 
     mediation_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        mediation_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mediation_id=mediation_id,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 MediationIdMatchInfo.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/mediation_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     MediationList - a model defined in OpenAPI
         results: List of mediation records [Optional].
     """
 
     results: Optional[List[MediationRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[MediationRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 MediationList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_form_param.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,57 +4,35 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.menu_option import MenuOption
 
 
-class Menu(BaseModel):
+class MenuFormParam(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Menu - a model defined in OpenAPI
-        options: List of menu options.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
-        description: Introductory text for the menu [Optional].
-        errormsg: An optional error message to display in menu header [Optional].
-        title: Menu title [Optional].
+    MenuFormParam - a model defined in OpenAPI
+        name: Menu parameter name.
+        title: Menu parameter title.
+        default: Default parameter value [Optional].
+        description: Additional descriptive text for menu form parameter [Optional].
+        required: Whether parameter is required [Optional].
+        type: Menu form parameter input type [Optional].
     """
 
-    options: List[MenuOption]
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
+    name: str
+    title: str
+    default: Optional[str] = None
     description: Optional[str] = None
-    errormsg: Optional[str] = None
-    title: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        options: List[MenuOption] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        description: Optional[str] = None,
-        errormsg: Optional[str] = None,
-        title: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            description=description,
-            errormsg=errormsg,
-            options=options,
-            title=title,
-            **kwargs,
-        )
+    required: Optional[bool] = None
+    type: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Menu.update_forward_refs()
+MenuFormParam.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_form.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/submission_requirements.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,49 +4,39 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.menu_form_param import MenuFormParam
 
 
-class MenuForm(BaseModel):
+class SubmissionRequirements(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    MenuForm - a model defined in OpenAPI
-        description: Additional descriptive text for menu form [Optional].
-        params: List of form parameters [Optional].
-        submit_label: Alternative label for form submit button [Optional].
-        title: Menu form title [Optional].
+    SubmissionRequirements - a model defined in OpenAPI
+        count: Count Value [Optional].
+        from_: From [Optional].
+        from_nested: The from_nested of this SubmissionRequirements [Optional].
+        max: Max Value [Optional].
+        min: Min Value [Optional].
+        name: Name [Optional].
+        purpose: Purpose [Optional].
+        rule: Selection [Optional].
     """
 
-    description: Optional[str] = None
-    params: Optional[List[MenuFormParam]] = None
-    submit_label: Optional[str] = Field(None, alias="submit-label")
-    title: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        description: Optional[str] = None,
-        params: Optional[List[MenuFormParam]] = None,
-        submit_label: Optional[str] = None,
-        title: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            description=description,
-            params=params,
-            submit_label=submit_label,
-            title=title,
-            **kwargs,
-        )
+    count: Optional[int] = None
+    from_: Optional[str] = Field(None, alias="from")
+    from_nested: Optional[List[SubmissionRequirements]] = None
+    max: Optional[int] = None
+    min: Optional[int] = None
+    name: Optional[str] = None
+    purpose: Optional[str] = None
+    rule: Optional[Literal["all", "pick"]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-MenuForm.update_forward_refs()
+SubmissionRequirements.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/menu_json.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/menu_json.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,29 +24,12 @@
     """
 
     options: List[MenuOption]
     description: Optional[str] = None
     errormsg: Optional[str] = None
     title: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        options: List[MenuOption] = None,
-        description: Optional[str] = None,
-        errormsg: Optional[str] = None,
-        title: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            description=description,
-            errormsg=errormsg,
-            options=options,
-            title=title,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 MenuJson.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/model_schema.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_filter_indy.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,99 +6,98 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ModelSchema(BaseModel):
+class V20CredFilterIndy(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ModelSchema - a model defined in OpenAPI
-        attr_names: Schema attribute names [Optional].
-        id: Schema identifier [Optional].
-        name: Schema name [Optional].
-        seq_no: Schema sequence number [Optional].
-        ver: Node protocol version [Optional].
-        version: Schema version [Optional].
+    V20CredFilterIndy - a model defined in OpenAPI
+        cred_def_id: Credential definition identifier [Optional].
+        issuer_did: Credential issuer DID [Optional].
+        schema_id: Schema identifier [Optional].
+        schema_issuer_did: Schema issuer DID [Optional].
+        schema_name: Schema name [Optional].
+        schema_version: Schema version [Optional].
     """
 
-    attr_names: Optional[List[str]] = Field(None, alias="attrNames")
-    id: Optional[str] = None
-    name: Optional[str] = None
-    seq_no: Optional[int] = Field(None, alias="seqNo")
-    ver: Optional[str] = None
-    version: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        attr_names: Optional[List[str]] = None,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        seq_no: Optional[int] = None,
-        ver: Optional[str] = None,
-        version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attr_names=attr_names,
-            id=id,
-            name=name,
-            seq_no=seq_no,
-            ver=ver,
-            version=version,
-            **kwargs,
-        )
+    cred_def_id: Optional[str] = None
+    issuer_did: Optional[str] = None
+    schema_id: Optional[str] = None
+    schema_issuer_did: Optional[str] = None
+    schema_name: Optional[str] = None
+    schema_version: Optional[str] = None
 
-    @validator("id")
-    def id_pattern(cls, value):
+    @validator("cred_def_id")
+    def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of id does not match regex pattern ('{pattern}')")
+            raise ValueError(
+                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
+            )
         return value
 
-    @validator("seq_no")
-    def seq_no_min(cls, value):
+    @validator("issuer_did")
+    def issuer_did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        if value < 1:
-            raise ValueError(f"seq_no must be greater than 1, currently {value}")
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of issuer_did does not match regex pattern ('{pattern}')"
+            )
         return value
 
-    @validator("ver")
-    def ver_pattern(cls, value):
+    @validator("schema_id")
+    def schema_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[0-9.]+$"
+        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
         if not re.match(pattern, value):
-            raise ValueError(f"Value of ver does not match regex pattern ('{pattern}')")
+            raise ValueError(
+                f"Value of schema_id does not match regex pattern ('{pattern}')"
+            )
+        return value
+
+    @validator("schema_issuer_did")
+    def schema_issuer_did_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of schema_issuer_did does not match regex pattern ('{pattern}')"
+            )
         return value
 
-    @validator("version")
-    def version_pattern(cls, value):
+    @validator("schema_version")
+    def schema_version_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^[0-9.]+$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of version does not match regex pattern ('{pattern}')"
+                f"Value of schema_version does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-ModelSchema.update_forward_refs()
+V20CredFilterIndy.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/oob_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_create.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,124 +4,109 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.invitation_message import InvitationMessage
-from aries_cloudcontroller.model.service_decorator import ServiceDecorator
+from aries_cloudcontroller.model.credential_preview import CredentialPreview
 
 
-class OobRecord(BaseModel):
+class V10CredentialCreate(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    OobRecord - a model defined in OpenAPI
-        invi_msg_id: Invitation message identifier.
-        invitation: Out of band invitation message.
-        oob_id: Oob record identifier.
-        state: Out of band message exchange state.
-        attach_thread_id: Connection record identifier [Optional].
-        connection_id: Connection record identifier [Optional].
-        created_at: Time of record creation [Optional].
-        our_recipient_key: Recipient key used for oob invitation [Optional].
-        role: OOB Role [Optional].
-        their_service: The their_service of this OobRecord [Optional].
+    V10CredentialCreate - a model defined in OpenAPI
+        credential_proposal: The credential_proposal of this V10CredentialCreate.
+        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
+        comment: Human-readable comment [Optional].
+        cred_def_id: Credential definition identifier [Optional].
+        issuer_did: Credential issuer DID [Optional].
+        schema_id: Schema identifier [Optional].
+        schema_issuer_did: Schema issuer DID [Optional].
+        schema_name: Schema name [Optional].
+        schema_version: Schema version [Optional].
         trace: Record trace information, based on agent configuration [Optional].
-        updated_at: Time of last record update [Optional].
     """
 
-    invi_msg_id: str
-    invitation: InvitationMessage
-    oob_id: str
-    state: Literal[
-        "initial",
-        "prepare-response",
-        "await-response",
-        "reuse-not-accepted",
-        "reuse-accepted",
-        "done",
-        "deleted",
-    ]
-    attach_thread_id: Optional[str] = None
-    connection_id: Optional[str] = None
-    created_at: Optional[str] = None
-    our_recipient_key: Optional[str] = None
-    role: Optional[Literal["sender", "receiver"]] = None
-    their_service: Optional[ServiceDecorator] = None
+    credential_proposal: CredentialPreview
+    auto_remove: Optional[bool] = None
+    comment: Optional[str] = None
+    cred_def_id: Optional[str] = None
+    issuer_did: Optional[str] = None
+    schema_id: Optional[str] = None
+    schema_issuer_did: Optional[str] = None
+    schema_name: Optional[str] = None
+    schema_version: Optional[str] = None
     trace: Optional[bool] = None
-    updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        invi_msg_id: str = None,
-        invitation: InvitationMessage = None,
-        oob_id: str = None,
-        state: Literal[
-            "initial",
-            "prepare-response",
-            "await-response",
-            "reuse-not-accepted",
-            "reuse-accepted",
-            "done",
-            "deleted",
-        ] = None,
-        attach_thread_id: Optional[str] = None,
-        connection_id: Optional[str] = None,
-        created_at: Optional[str] = None,
-        our_recipient_key: Optional[str] = None,
-        role: Optional[Literal["sender", "receiver"]] = None,
-        their_service: Optional[ServiceDecorator] = None,
-        trace: Optional[bool] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attach_thread_id=attach_thread_id,
-            connection_id=connection_id,
-            created_at=created_at,
-            invi_msg_id=invi_msg_id,
-            invitation=invitation,
-            oob_id=oob_id,
-            our_recipient_key=our_recipient_key,
-            role=role,
-            state=state,
-            their_service=their_service,
-            trace=trace,
-            updated_at=updated_at,
-            **kwargs,
-        )
+    @validator("cred_def_id")
+    def cred_def_id_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of cred_def_id does not match regex pattern ('{pattern}')"
+            )
+        return value
+
+    @validator("issuer_did")
+    def issuer_did_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of issuer_did does not match regex pattern ('{pattern}')"
+            )
+        return value
+
+    @validator("schema_id")
+    def schema_id_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of schema_id does not match regex pattern ('{pattern}')"
+            )
+        return value
 
-    @validator("created_at")
-    def created_at_pattern(cls, value):
+    @validator("schema_issuer_did")
+    def schema_issuer_did_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of created_at does not match regex pattern ('{pattern}')"
+                f"Value of schema_issuer_did does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("updated_at")
-    def updated_at_pattern(cls, value):
+    @validator("schema_version")
+    def schema_version_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        pattern = r"^[0-9.]+$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of updated_at does not match regex pattern ('{pattern}')"
+                f"Value of schema_version does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-OobRecord.update_forward_refs()
+V10CredentialCreate.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/perform_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/perform_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         name: Menu option name [Optional].
         params: Input parameter values [Optional].
     """
 
     name: Optional[str] = None
     params: Optional[Dict[str, str]] = None
 
-    def __init__(
-        self,
-        *,
-        name: Optional[str] = None,
-        params: Optional[Dict[str, str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            name=name,
-            params=params,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 PerformRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ping_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ping_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     PingRequest - a model defined in OpenAPI
         comment: Comment for the ping message [Optional].
     """
 
     comment: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            comment=comment,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 PingRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/ping_request_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/protocol_descriptor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class PingRequestResponse(BaseModel):
+class ProtocolDescriptor(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    PingRequestResponse - a model defined in OpenAPI
-        thread_id: Thread ID of the ping message [Optional].
+    ProtocolDescriptor - a model defined in OpenAPI
+        pid: The pid of this ProtocolDescriptor.
+        roles: List of roles [Optional].
     """
 
-    thread_id: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        thread_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            thread_id=thread_id,
-            **kwargs,
-        )
+    pid: str
+    roles: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-PingRequestResponse.update_forward_refs()
+ProtocolDescriptor.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_definition.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_definition.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,35 +30,14 @@
     format: Optional[ClaimFormat] = None
     id: Optional[str] = None
     input_descriptors: Optional[List[InputDescriptors]] = None
     name: Optional[str] = None
     purpose: Optional[str] = None
     submission_requirements: Optional[List[SubmissionRequirements]] = None
 
-    def __init__(
-        self,
-        *,
-        format: Optional[ClaimFormat] = None,
-        id: Optional[str] = None,
-        input_descriptors: Optional[List[InputDescriptors]] = None,
-        name: Optional[str] = None,
-        purpose: Optional[str] = None,
-        submission_requirements: Optional[List[SubmissionRequirements]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            format=format,
-            id=id,
-            input_descriptors=input_descriptors,
-            name=name,
-            purpose=purpose,
-            submission_requirements=submission_requirements,
-            **kwargs,
-        )
-
     @validator("id")
     def id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-4[a-fA-F0-9]{3}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_proposal.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,29 +24,12 @@
     """
 
     presentation_proposal: IndyPresPreview
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        presentation_proposal: IndyPresPreview = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            presentation_proposal=presentation_proposal,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 PresentationProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/presentation_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_proposal_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,51 +4,34 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attach_decorator import AttachDecorator
+from aries_cloudcontroller.model.indy_pres_preview import IndyPresPreview
 
 
-class PresentationRequest(BaseModel):
+class V10PresentationProposalRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    PresentationRequest - a model defined in OpenAPI
-        request_presentationsattach: The request_presentationsattach of this PresentationRequest.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
+    V10PresentationProposalRequest - a model defined in OpenAPI
+        connection_id: Connection identifier.
+        presentation_proposal: The presentation_proposal of this V10PresentationProposalRequest.
+        auto_present: Whether to respond automatically to presentation requests, building and presenting requested proof [Optional].
         comment: Human-readable comment [Optional].
+        trace: Whether to trace event (default false) [Optional].
     """
 
-    request_presentationsattach: List[AttachDecorator] = Field(
-        ..., alias="request_presentations~attach"
-    )
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
+    connection_id: str
+    presentation_proposal: IndyPresPreview
+    auto_present: Optional[bool] = None
     comment: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        request_presentationsattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            request_presentationsattach=request_presentationsattach,
-            **kwargs,
-        )
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-PresentationRequest.update_forward_refs()
+V10PresentationProposalRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/protocol_descriptor.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/keylist_query_filter_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,38 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ProtocolDescriptor(BaseModel):
+class KeylistQueryFilterRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ProtocolDescriptor - a model defined in OpenAPI
-        pid: The pid of this ProtocolDescriptor.
-        roles: List of roles [Optional].
+    KeylistQueryFilterRequest - a model defined in OpenAPI
+        filter: Filter for keylist query [Optional].
     """
 
-    pid: str
-    roles: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        pid: str = None,
-        roles: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            pid=pid,
-            roles=roles,
-            **kwargs,
-        )
+    filter: Optional[Dict[str, Any]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-ProtocolDescriptor.update_forward_refs()
+KeylistQueryFilterRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/publish_revocations.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/query_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class PublishRevocations(BaseModel):
+class QueryItem(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    PublishRevocations - a model defined in OpenAPI
-        rrid2crid: Credential revocation ids by revocation registry id [Optional].
+    QueryItem - a model defined in OpenAPI
+        feature_type: feature type.
+        match: match.
     """
 
-    rrid2crid: Optional[Dict[str, List[str]]] = None
-
-    def __init__(
-        self,
-        *,
-        rrid2crid: Optional[Dict[str, List[str]]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            rrid2crid=rrid2crid,
-            **kwargs,
-        )
+    feature_type: Literal["protocol", "goal-code"] = Field(..., alias="feature-type")
+    match: str
 
     class Config:
         allow_population_by_field_name = True
 
 
-PublishRevocations.update_forward_refs()
+QueryItem.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/queries.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/presentation_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,45 +4,34 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.query_item import QueryItem
+from aries_cloudcontroller.model.attach_decorator import AttachDecorator
 
 
-class Queries(BaseModel):
+class PresentationRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Queries - a model defined in OpenAPI
+    PresentationRequest - a model defined in OpenAPI
+        request_presentationsattach: The request_presentationsattach of this PresentationRequest.
         id: Message identifier [Optional].
         type: Message type [Optional].
-        queries: The queries of this Queries [Optional].
+        comment: Human-readable comment [Optional].
     """
 
+    request_presentationsattach: List[AttachDecorator] = Field(
+        ..., alias="request_presentations~attach"
+    )
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
-    queries: Optional[List[QueryItem]] = None
-
-    def __init__(
-        self,
-        *,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        queries: Optional[List[QueryItem]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            queries=queries,
-            **kwargs,
-        )
+    comment: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Queries.update_forward_refs()
+PresentationRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/query.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/mediation_deny.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,46 +6,29 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class Query(BaseModel):
+class MediationDeny(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    Query - a model defined in OpenAPI
-        query: The query of this Query.
+    MediationDeny - a model defined in OpenAPI
         id: Message identifier [Optional].
         type: Message type [Optional].
-        comment: The comment of this Query [Optional].
+        mediator_terms: The mediator_terms of this MediationDeny [Optional].
+        recipient_terms: The recipient_terms of this MediationDeny [Optional].
     """
 
-    query: str
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
-    comment: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        query: str = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            query=query,
-            **kwargs,
-        )
+    mediator_terms: Optional[List[str]] = None
+    recipient_terms: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-Query.update_forward_refs()
+MediationDeny.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/query_item.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_regs_created.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,38 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class QueryItem(BaseModel):
+class RevRegsCreated(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    QueryItem - a model defined in OpenAPI
-        feature_type: feature type.
-        match: match.
+    RevRegsCreated - a model defined in OpenAPI
+        rev_reg_ids: The rev_reg_ids of this RevRegsCreated [Optional].
     """
 
-    feature_type: Literal["protocol", "goal-code"] = Field(..., alias="feature-type")
-    match: str
-
-    def __init__(
-        self,
-        *,
-        feature_type: Literal["protocol", "goal-code"] = None,
-        match: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            feature_type=feature_type,
-            match=match,
-            **kwargs,
-        )
+    rev_reg_ids: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-QueryItem.update_forward_refs()
+RevRegsCreated.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/raw_encoded.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/raw_encoded.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         encoded: Encoded value [Optional].
         raw: Raw value [Optional].
     """
 
     encoded: Optional[str] = None
     raw: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        encoded: Optional[str] = None,
-        raw: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            encoded=encoded,
-            raw=raw,
-            **kwargs,
-        )
-
     @validator("encoded")
     def encoded_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^-?[0-9]*$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/remove_wallet_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_problem_report_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class RemoveWalletRequest(BaseModel):
+class V10CredentialProblemReportRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    RemoveWalletRequest - a model defined in OpenAPI
-        wallet_key: Master key used for key derivation. Only required for             unmanaged wallets. [Optional].
+    V10CredentialProblemReportRequest - a model defined in OpenAPI
+        description: The description of this V10CredentialProblemReportRequest.
     """
 
-    wallet_key: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        wallet_key: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            wallet_key=wallet_key,
-            **kwargs,
-        )
+    description: str
 
     class Config:
         allow_population_by_field_name = True
 
 
-RemoveWalletRequest.update_forward_refs()
+V10CredentialProblemReportRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/resolution_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_record.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,38 +6,27 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class ResolutionResult(BaseModel):
+class TAARecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    ResolutionResult - a model defined in OpenAPI
-        did_document: DID Document.
-        metadata: Resolution metadata.
+    TAARecord - a model defined in OpenAPI
+        digest: The digest of this TAARecord [Optional].
+        text: The text of this TAARecord [Optional].
+        version: The version of this TAARecord [Optional].
     """
 
-    did_document: Dict[str, Any]
-    metadata: Dict[str, Any]
-
-    def __init__(
-        self,
-        *,
-        did_document: Dict[str, Any] = None,
-        metadata: Dict[str, Any] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            did_document=did_document,
-            metadata=metadata,
-            **kwargs,
-        )
+    digest: Optional[str] = None
+    text: Optional[str] = None
+    version: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-ResolutionResult.update_forward_refs()
+TAARecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_create_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_create_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         credential_definition_id: Credential definition identifier [Optional].
         max_cred_num: Revocation registry size [Optional].
     """
 
     credential_definition_id: Optional[str] = None
     max_cred_num: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        credential_definition_id: Optional[str] = None,
-        max_cred_num: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_definition_id=credential_definition_id,
-            max_cred_num=max_cred_num,
-            **kwargs,
-        )
-
     @validator("credential_definition_id")
     def credential_definition_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_issued_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_issued_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,14 @@
 
     RevRegIssuedResult - a model defined in OpenAPI
         result: Number of credentials issued against revocation registry [Optional].
     """
 
     result: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        result: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
-
     @validator("result")
     def result_min(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value < 0:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_get_result.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.issuer_rev_reg_record import IssuerRevRegRecord
+from aries_cloudcontroller.model.model_schema import ModelSchema
 
 
-class RevRegResult(BaseModel):
+class SchemaGetResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    RevRegResult - a model defined in OpenAPI
-        result: The result of this RevRegResult [Optional].
+    SchemaGetResult - a model defined in OpenAPI
+        schema_: The schema_ of this SchemaGetResult [Optional].
     """
 
-    result: Optional[IssuerRevRegRecord] = None
-
-    def __init__(
-        self,
-        *,
-        result: Optional[IssuerRevRegRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
+    schema_: Optional[ModelSchema] = Field(None, alias="schema")
 
     class Config:
         allow_population_by_field_name = True
 
 
-RevRegResult.update_forward_refs()
+SchemaGetResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_update_tails_file_uri.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/endorser_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class RevRegUpdateTailsFileUri(BaseModel):
+class EndorserInfo(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    RevRegUpdateTailsFileUri - a model defined in OpenAPI
-        tails_public_uri: Public URI to the tails file.
+    EndorserInfo - a model defined in OpenAPI
+        endorser_did: Endorser DID.
+        endorser_name: Endorser Name [Optional].
     """
 
-    tails_public_uri: str
-
-    def __init__(
-        self,
-        *,
-        tails_public_uri: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            tails_public_uri=tails_public_uri,
-            **kwargs,
-        )
+    endorser_did: str
+    endorser_name: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-RevRegUpdateTailsFileUri.update_forward_refs()
+EndorserInfo.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/rev_reg_wallet_updated_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         rev_reg_delta: Indy revocation registry delta [Optional].
     """
 
     accum_calculated: Optional[Dict[str, Any]] = None
     accum_fixed: Optional[Dict[str, Any]] = None
     rev_reg_delta: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        accum_calculated: Optional[Dict[str, Any]] = None,
-        accum_fixed: Optional[Dict[str, Any]] = None,
-        rev_reg_delta: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            accum_calculated=accum_calculated,
-            accum_fixed=accum_fixed,
-            rev_reg_delta=rev_reg_delta,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 RevRegWalletUpdatedResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/rev_regs_created.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schemas_created_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class RevRegsCreated(BaseModel):
+class SchemasCreatedResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    RevRegsCreated - a model defined in OpenAPI
-        rev_reg_ids: The rev_reg_ids of this RevRegsCreated [Optional].
+    SchemasCreatedResult - a model defined in OpenAPI
+        schema_ids: The schema_ids of this SchemasCreatedResult [Optional].
     """
 
-    rev_reg_ids: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        rev_reg_ids: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            rev_reg_ids=rev_reg_ids,
-            **kwargs,
-        )
+    schema_ids: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-RevRegsCreated.update_forward_refs()
+SchemasCreatedResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/revoke_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/revoke_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,41 +33,14 @@
     cred_rev_id: Optional[str] = None
     notify: Optional[bool] = None
     notify_version: Optional[Literal["v1_0", "v2_0"]] = None
     publish: Optional[bool] = None
     rev_reg_id: Optional[str] = None
     thread_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        comment: Optional[str] = None,
-        connection_id: Optional[str] = None,
-        cred_ex_id: Optional[str] = None,
-        cred_rev_id: Optional[str] = None,
-        notify: Optional[bool] = None,
-        notify_version: Optional[Literal["v1_0", "v2_0"]] = None,
-        publish: Optional[bool] = None,
-        rev_reg_id: Optional[str] = None,
-        thread_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            comment=comment,
-            connection_id=connection_id,
-            cred_ex_id=cred_ex_id,
-            cred_rev_id=cred_rev_id,
-            notify=notify,
-            notify_version=notify_version,
-            publish=publish,
-            rev_reg_id=rev_reg_id,
-            thread_id=thread_id,
-            **kwargs,
-        )
-
     @validator("connection_id")
     def connection_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-4[a-fA-F0-9]{3}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/route_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/route_record.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,39 +31,14 @@
     created_at: Optional[str] = None
     record_id: Optional[str] = None
     role: Optional[str] = None
     state: Optional[str] = None
     updated_at: Optional[str] = None
     wallet_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        recipient_key: str = None,
-        connection_id: Optional[str] = None,
-        created_at: Optional[str] = None,
-        record_id: Optional[str] = None,
-        role: Optional[str] = None,
-        state: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        wallet_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            connection_id=connection_id,
-            created_at=created_at,
-            recipient_key=recipient_key,
-            record_id=record_id,
-            role=role,
-            state=state,
-            updated_at=updated_at,
-            wallet_id=wallet_id,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_get_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_format.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.model_schema import ModelSchema
 
 
-class SchemaGetResult(BaseModel):
+class V20PresFormat(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SchemaGetResult - a model defined in OpenAPI
-        schema_: The schema_ of this SchemaGetResult [Optional].
+    V20PresFormat - a model defined in OpenAPI
+        attach_id: Attachment identifier.
+        format: Attachment format specifier.
     """
 
-    schema_: Optional[ModelSchema] = Field(None, alias="schema")
-
-    def __init__(
-        self,
-        *,
-        schema_: Optional[ModelSchema] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            schema_=schema_,
-            **kwargs,
-        )
+    attach_id: str
+    format: str
 
     class Config:
         allow_population_by_field_name = True
 
 
-SchemaGetResult.update_forward_refs()
+V20PresFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_input_descriptor.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/service_decorator.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,38 +6,27 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class SchemaInputDescriptor(BaseModel):
+class ServiceDecorator(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SchemaInputDescriptor - a model defined in OpenAPI
-        required: Required [Optional].
-        uri: URI [Optional].
+    ServiceDecorator - a model defined in OpenAPI
+        recipient_keys: List of recipient keys [Optional].
+        service_endpoint: Service endpoint at which to reach this agent [Optional].
+        routing_keys: List of routing keys [Optional].
     """
 
-    required: Optional[bool] = None
-    uri: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        required: Optional[bool] = None,
-        uri: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            required=required,
-            uri=uri,
-            **kwargs,
-        )
+    recipient_keys: Optional[List[str]] = Field(None, alias="recipientKeys")
+    service_endpoint: Optional[str] = Field(None, alias="serviceEndpoint")
+    routing_keys: Optional[List[str]] = Field(None, alias="routingKeys")
 
     class Config:
         allow_population_by_field_name = True
 
 
-SchemaInputDescriptor.update_forward_refs()
+ServiceDecorator.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_send_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_send_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,29 +21,14 @@
         schema_version: Schema version.
     """
 
     attributes: List[str]
     schema_name: str
     schema_version: str
 
-    def __init__(
-        self,
-        *,
-        attributes: List[str] = None,
-        schema_name: str = None,
-        schema_version: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attributes=attributes,
-            schema_name=schema_name,
-            schema_version=schema_version,
-            **kwargs,
-        )
-
     @validator("schema_version")
     def schema_version_pattern(cls, value):
         pattern = r"^[0-9.]+$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of schema_version does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schema_send_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/schema_send_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,27 +20,14 @@
         schema_id: Schema identifier.
         schema_: Schema definition [Optional].
     """
 
     schema_id: str
     schema_: Optional[ModelSchema] = Field(None, alias="schema")
 
-    def __init__(
-        self,
-        *,
-        schema_id: str = None,
-        schema_: Optional[ModelSchema] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            schema_=schema_,
-            schema_id=schema_id,
-            **kwargs,
-        )
-
     @validator("schema_id")
     def schema_id_pattern(cls, value):
         pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of schema_id does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/schemas_created_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_issue_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class SchemasCreatedResult(BaseModel):
+class V10CredentialIssueRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SchemasCreatedResult - a model defined in OpenAPI
-        schema_ids: The schema_ids of this SchemasCreatedResult [Optional].
+    V10CredentialIssueRequest - a model defined in OpenAPI
+        comment: Human-readable comment [Optional].
     """
 
-    schema_ids: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        schema_ids: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            schema_ids=schema_ids,
-            **kwargs,
-        )
+    comment: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-SchemasCreatedResult.update_forward_refs()
+V10CredentialIssueRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/send_menu.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/verify_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,37 +4,27 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.menu_json import MenuJson
 
 
-class SendMenu(BaseModel):
+class VerifyResponse(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SendMenu - a model defined in OpenAPI
-        menu: Menu to send to connection.
+    VerifyResponse - a model defined in OpenAPI
+        valid: The valid of this VerifyResponse.
+        error: Error text [Optional].
     """
 
-    menu: MenuJson
-
-    def __init__(
-        self,
-        *,
-        menu: MenuJson = None,
-        **kwargs,
-    ):
-        super().__init__(
-            menu=menu,
-            **kwargs,
-        )
+    valid: bool
+    error: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-SendMenu.update_forward_refs()
+VerifyResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/send_message.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_format.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,34 +6,25 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class SendMessage(BaseModel):
+class V20CredFormat(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SendMessage - a model defined in OpenAPI
-        content: Message content [Optional].
+    V20CredFormat - a model defined in OpenAPI
+        attach_id: Attachment identifier.
+        format: Attachment format specifier.
     """
 
-    content: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        content: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            content=content,
-            **kwargs,
-        )
+    attach_id: str
+    format: str
 
     class Config:
         allow_population_by_field_name = True
 
 
-SendMessage.update_forward_refs()
+V20CredFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/sign_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/sign_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,25 +20,12 @@
         doc: The doc of this SignRequest.
         verkey: Verkey to use for signing.
     """
 
     doc: Doc
     verkey: str
 
-    def __init__(
-        self,
-        *,
-        doc: Doc = None,
-        verkey: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            doc=doc,
-            verkey=verkey,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 SignRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/sign_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/sign_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         error: Error text [Optional].
         signed_doc: Signed document [Optional].
     """
 
     error: Optional[str] = None
     signed_doc: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        error: Optional[str] = None,
-        signed_doc: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            error=error,
-            signed_doc=signed_doc,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 SignResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/signature_options.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/signature_options.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,31 +25,12 @@
 
     proof_purpose: str = Field(..., alias="proofPurpose")
     verification_method: str = Field(..., alias="verificationMethod")
     challenge: Optional[str] = None
     domain: Optional[str] = None
     type: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        proof_purpose: str = None,
-        verification_method: str = None,
-        challenge: Optional[str] = None,
-        domain: Optional[str] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            challenge=challenge,
-            domain=domain,
-            proof_purpose=proof_purpose,
-            type=type,
-            verification_method=verification_method,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 SignatureOptions.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/signed_doc.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.signature_options import SignatureOptions
+from aries_cloudcontroller.model.taa_info import TAAInfo
 
 
-class SignedDoc(BaseModel):
+class TAAResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    SignedDoc - a model defined in OpenAPI
-        proof: Linked data proof.
+    TAAResult - a model defined in OpenAPI
+        result: The result of this TAAResult [Optional].
     """
 
-    proof: SignatureOptions
-
-    def __init__(
-        self,
-        *,
-        proof: SignatureOptions = None,
-        **kwargs,
-    ):
-        super().__init__(
-            proof=proof,
-            **kwargs,
-        )
+    result: Optional[TAAInfo] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-SignedDoc.update_forward_refs()
+TAAResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_accept.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_accept.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         version: The version of this TAAAccept [Optional].
     """
 
     mechanism: Optional[str] = None
     text: Optional[str] = None
     version: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        mechanism: Optional[str] = None,
-        text: Optional[str] = None,
-        version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mechanism=mechanism,
-            text=text,
-            version=version,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TAAAccept.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_acceptance.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_acceptance.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,27 +19,14 @@
         mechanism: The mechanism of this TAAAcceptance [Optional].
         time: The time of this TAAAcceptance [Optional].
     """
 
     mechanism: Optional[str] = None
     time: Optional[int] = None
 
-    def __init__(
-        self,
-        *,
-        mechanism: Optional[str] = None,
-        time: Optional[int] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mechanism=mechanism,
-            time=time,
-            **kwargs,
-        )
-
     @validator("time")
     def time_max(cls, value):
         # Property is optional
         if value is None:
             return
 
         if value > 18446744073709551615:
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_info.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/taa_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,29 +26,12 @@
     """
 
     aml_record: Optional[AMLRecord] = None
     taa_accepted: Optional[TAAAcceptance] = None
     taa_record: Optional[TAARecord] = None
     taa_required: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        aml_record: Optional[AMLRecord] = None,
-        taa_accepted: Optional[TAAAcceptance] = None,
-        taa_record: Optional[TAARecord] = None,
-        taa_required: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            aml_record=aml_record,
-            taa_accepted=taa_accepted,
-            taa_record=taa_record,
-            taa_required=taa_required,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TAAInfo.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/taa_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_discovery_exchange_list_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.taa_info import TAAInfo
+from aries_cloudcontroller.model.v20_discovery_record import V20DiscoveryRecord
 
 
-class TAAResult(BaseModel):
+class V20DiscoveryExchangeListResult(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    TAAResult - a model defined in OpenAPI
-        result: The result of this TAAResult [Optional].
+    V20DiscoveryExchangeListResult - a model defined in OpenAPI
+        results: The results of this V20DiscoveryExchangeListResult [Optional].
     """
 
-    result: Optional[TAAInfo] = None
-
-    def __init__(
-        self,
-        *,
-        result: Optional[TAAInfo] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            result=result,
-            **kwargs,
-        )
+    results: Optional[List[V20DiscoveryRecord]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-TAAResult.update_forward_refs()
+V20DiscoveryExchangeListResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/tails_delete_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class TailsDeleteResponse(BaseModel):
+class V20CredIssueRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    TailsDeleteResponse - a model defined in OpenAPI
-        message: The message of this TailsDeleteResponse [Optional].
+    V20CredIssueRequest - a model defined in OpenAPI
+        comment: Human-readable comment [Optional].
     """
 
-    message: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        message: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            message=message,
-            **kwargs,
-        )
+    comment: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-TailsDeleteResponse.update_forward_refs()
+V20CredIssueRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/transaction_jobs.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_jobs.py`

 * *Files 25% similar despite different names*

```diff
@@ -23,29 +23,12 @@
     transaction_my_job: Optional[
         Literal["TRANSACTION_AUTHOR", "TRANSACTION_ENDORSER", "reset"]
     ] = None
     transaction_their_job: Optional[
         Literal["TRANSACTION_AUTHOR", "TRANSACTION_ENDORSER", "reset"]
     ] = None
 
-    def __init__(
-        self,
-        *,
-        transaction_my_job: Optional[
-            Literal["TRANSACTION_AUTHOR", "TRANSACTION_ENDORSER", "reset"]
-        ] = None,
-        transaction_their_job: Optional[
-            Literal["TRANSACTION_AUTHOR", "TRANSACTION_ENDORSER", "reset"]
-        ] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            transaction_my_job=transaction_my_job,
-            transaction_their_job=transaction_their_job,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TransactionJobs.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/transaction_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/transaction_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     TransactionList - a model defined in OpenAPI
         results: List of transaction records [Optional].
     """
 
     results: Optional[List[TransactionRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[TransactionRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TransactionList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_publish_revocations_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_publish_revocations_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         sent: The sent of this TxnOrPublishRevocationsResult [Optional].
         txn: Revocation registry revocations transaction to endorse [Optional].
     """
 
     sent: Optional[PublishRevocations] = None
     txn: Optional[TransactionRecord] = None
 
-    def __init__(
-        self,
-        *,
-        sent: Optional[PublishRevocations] = None,
-        txn: Optional[TransactionRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            sent=sent,
-            txn=txn,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TxnOrPublishRevocationsResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_register_ledger_nym_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,25 +20,12 @@
         success: Success of nym registration operation [Optional].
         txn: DID transaction to endorse [Optional].
     """
 
     success: Optional[bool] = None
     txn: Optional[TransactionRecord] = None
 
-    def __init__(
-        self,
-        *,
-        success: Optional[bool] = None,
-        txn: Optional[TransactionRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            success=success,
-            txn=txn,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TxnOrRegisterLedgerNymResponse.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_rev_reg_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_rev_reg_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         sent: The sent of this TxnOrRevRegResult [Optional].
         txn: Revocation registry definition transaction to endorse [Optional].
     """
 
     sent: Optional[RevRegResult] = None
     txn: Optional[TransactionRecord] = None
 
-    def __init__(
-        self,
-        *,
-        sent: Optional[RevRegResult] = None,
-        txn: Optional[TransactionRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            sent=sent,
-            txn=txn,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TxnOrRevRegResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/txn_or_schema_send_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/txn_or_schema_send_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         sent: Content sent [Optional].
         txn: Schema transaction to endorse [Optional].
     """
 
     sent: Optional[SchemaSendResult] = None
     txn: Optional[TransactionRecord] = None
 
-    def __init__(
-        self,
-        *,
-        sent: Optional[SchemaSendResult] = None,
-        txn: Optional[TransactionRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            sent=sent,
-            txn=txn,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 TxnOrSchemaSendResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/update_wallet_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/update_wallet_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,29 +23,12 @@
     """
 
     image_url: Optional[str] = None
     label: Optional[str] = None
     wallet_dispatch_type: Optional[Literal["default", "both", "base"]] = None
     wallet_webhook_urls: Optional[List[str]] = None
 
-    def __init__(
-        self,
-        *,
-        image_url: Optional[str] = None,
-        label: Optional[str] = None,
-        wallet_dispatch_type: Optional[Literal["default", "both", "base"]] = None,
-        wallet_webhook_urls: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            image_url=image_url,
-            label=label,
-            wallet_dispatch_type=wallet_dispatch_type,
-            wallet_webhook_urls=wallet_webhook_urls,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 UpdateWalletRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_bound_offer_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_bound_offer_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V10CredentialBoundOfferRequest - a model defined in OpenAPI
         counter_proposal: Optional counter-proposal [Optional].
     """
 
     counter_proposal: Optional[CredentialProposal] = None
 
-    def __init__(
-        self,
-        *,
-        counter_proposal: Optional[CredentialProposal] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            counter_proposal=counter_proposal,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10CredentialBoundOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_conn_free_offer_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,35 +28,14 @@
     cred_def_id: str
     credential_preview: CredentialPreview
     auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        cred_def_id: str = None,
-        credential_preview: CredentialPreview = None,
-        auto_issue: Optional[bool] = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_issue=auto_issue,
-            auto_remove=auto_remove,
-            comment=comment,
-            cred_def_id=cred_def_id,
-            credential_preview=credential_preview,
-            trace=trace,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of cred_def_id does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_create.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_proposal_request_opt.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,72 +7,45 @@
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.credential_preview import CredentialPreview
 
 
-class V10CredentialCreate(BaseModel):
+class V10CredentialProposalRequestOpt(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10CredentialCreate - a model defined in OpenAPI
-        credential_proposal: The credential_proposal of this V10CredentialCreate.
+    V10CredentialProposalRequestOpt - a model defined in OpenAPI
+        connection_id: Connection identifier.
         auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
         cred_def_id: Credential definition identifier [Optional].
+        credential_proposal: The credential_proposal of this V10CredentialProposalRequestOpt [Optional].
         issuer_did: Credential issuer DID [Optional].
         schema_id: Schema identifier [Optional].
         schema_issuer_did: Schema issuer DID [Optional].
         schema_name: Schema name [Optional].
         schema_version: Schema version [Optional].
         trace: Record trace information, based on agent configuration [Optional].
     """
 
-    credential_proposal: CredentialPreview
+    connection_id: str
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     cred_def_id: Optional[str] = None
+    credential_proposal: Optional[CredentialPreview] = None
     issuer_did: Optional[str] = None
     schema_id: Optional[str] = None
     schema_issuer_did: Optional[str] = None
     schema_name: Optional[str] = None
     schema_version: Optional[str] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        credential_proposal: CredentialPreview = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        cred_def_id: Optional[str] = None,
-        issuer_did: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        schema_issuer_did: Optional[str] = None,
-        schema_name: Optional[str] = None,
-        schema_version: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_remove=auto_remove,
-            comment=comment,
-            cred_def_id=cred_def_id,
-            credential_proposal=credential_proposal,
-            issuer_did=issuer_did,
-            schema_id=schema_id,
-            schema_issuer_did=schema_issuer_did,
-            schema_name=schema_name,
-            schema_version=schema_version,
-            trace=trace,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
@@ -134,8 +107,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V10CredentialCreate.update_forward_refs()
+V10CredentialProposalRequestOpt.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_exchange_list_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_exchange_list_result.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V10CredentialExchangeListResult - a model defined in OpenAPI
         results: Aries#0036 v1.0 credential exchange records [Optional].
     """
 
     results: Optional[List[V10CredentialExchange]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[V10CredentialExchange]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10CredentialExchangeListResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_free_offer_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_free_offer_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,37 +30,14 @@
     cred_def_id: str
     credential_preview: CredentialPreview
     auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: str = None,
-        cred_def_id: str = None,
-        credential_preview: CredentialPreview = None,
-        auto_issue: Optional[bool] = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_issue=auto_issue,
-            auto_remove=auto_remove,
-            comment=comment,
-            connection_id=connection_id,
-            cred_def_id=cred_def_id,
-            credential_preview=credential_preview,
-            trace=trace,
-            **kwargs,
-        )
-
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+)):(.+)?$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of cred_def_id does not match regex pattern ('{pattern}')"
             )
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_issue_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/admin_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V10CredentialIssueRequest(BaseModel):
+class AdminConfig(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10CredentialIssueRequest - a model defined in OpenAPI
-        comment: Human-readable comment [Optional].
+    AdminConfig - a model defined in OpenAPI
+        config: Configuration settings [Optional].
     """
 
-    comment: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            comment=comment,
-            **kwargs,
-        )
+    config: Optional[Dict[str, Any]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V10CredentialIssueRequest.update_forward_refs()
+AdminConfig.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/issuer_rev_reg_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,78 +4,73 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.credential_preview import CredentialPreview
+from aries_cloudcontroller.model.indy_rev_reg_def import IndyRevRegDef
+from aries_cloudcontroller.model.indy_rev_reg_entry import IndyRevRegEntry
 
 
-class V10CredentialProposalRequestMand(BaseModel):
+class IssuerRevRegRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10CredentialProposalRequestMand - a model defined in OpenAPI
-        connection_id: Connection identifier.
-        credential_proposal: The credential_proposal of this V10CredentialProposalRequestMand.
-        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
-        comment: Human-readable comment [Optional].
+    IssuerRevRegRecord - a model defined in OpenAPI
+        created_at: Time of record creation [Optional].
         cred_def_id: Credential definition identifier [Optional].
-        issuer_did: Credential issuer DID [Optional].
-        schema_id: Schema identifier [Optional].
-        schema_issuer_did: Schema issuer DID [Optional].
-        schema_name: Schema name [Optional].
-        schema_version: Schema version [Optional].
-        trace: Record trace information, based on agent configuration [Optional].
+        error_msg: Error message [Optional].
+        issuer_did: Issuer DID [Optional].
+        max_cred_num: Maximum number of credentials for revocation registry [Optional].
+        pending_pub: Credential revocation identifier for credential revoked and pending publication to ledger [Optional].
+        record_id: Issuer revocation registry record identifier [Optional].
+        revoc_def_type: Revocation registry type (specify CL_ACCUM) [Optional].
+        revoc_reg_def: Revocation registry definition [Optional].
+        revoc_reg_entry: Revocation registry entry [Optional].
+        revoc_reg_id: Revocation registry identifier [Optional].
+        state: Issue revocation registry record state [Optional].
+        tag: Tag within issuer revocation registry identifier [Optional].
+        tails_hash: Tails hash [Optional].
+        tails_local_path: Local path to tails file [Optional].
+        tails_public_uri: Public URI for tails file [Optional].
+        updated_at: Time of last record update [Optional].
     """
 
-    connection_id: str
-    credential_proposal: CredentialPreview
-    auto_remove: Optional[bool] = None
-    comment: Optional[str] = None
+    created_at: Optional[str] = None
     cred_def_id: Optional[str] = None
+    error_msg: Optional[str] = None
     issuer_did: Optional[str] = None
-    schema_id: Optional[str] = None
-    schema_issuer_did: Optional[str] = None
-    schema_name: Optional[str] = None
-    schema_version: Optional[str] = None
-    trace: Optional[bool] = None
-
-    def __init__(
-        self,
-        *,
-        connection_id: str = None,
-        credential_proposal: CredentialPreview = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        cred_def_id: Optional[str] = None,
-        issuer_did: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        schema_issuer_did: Optional[str] = None,
-        schema_name: Optional[str] = None,
-        schema_version: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_remove=auto_remove,
-            comment=comment,
-            connection_id=connection_id,
-            cred_def_id=cred_def_id,
-            credential_proposal=credential_proposal,
-            issuer_did=issuer_did,
-            schema_id=schema_id,
-            schema_issuer_did=schema_issuer_did,
-            schema_name=schema_name,
-            schema_version=schema_version,
-            trace=trace,
-            **kwargs,
-        )
+    max_cred_num: Optional[int] = None
+    pending_pub: Optional[List[str]] = None
+    record_id: Optional[str] = None
+    revoc_def_type: Optional[Literal["CL_ACCUM"]] = None
+    revoc_reg_def: Optional[IndyRevRegDef] = None
+    revoc_reg_entry: Optional[IndyRevRegEntry] = None
+    revoc_reg_id: Optional[str] = None
+    state: Optional[str] = None
+    tag: Optional[str] = None
+    tails_hash: Optional[str] = None
+    tails_local_path: Optional[str] = None
+    tails_public_uri: Optional[str] = None
+    updated_at: Optional[str] = None
+
+    @validator("created_at")
+    def created_at_pattern(cls, value):
+        # Property is optional
+        if value is None:
+            return
+
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
+        if not re.match(pattern, value):
+            raise ValueError(
+                f"Value of created_at does not match regex pattern ('{pattern}')"
+            )
+        return value
 
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
@@ -95,51 +90,53 @@
         pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of issuer_did does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("schema_id")
-    def schema_id_pattern(cls, value):
+    @validator("revoc_reg_id")
+    def revoc_reg_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+$"
+        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of schema_id does not match regex pattern ('{pattern}')"
+                f"Value of revoc_reg_id does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("schema_issuer_did")
-    def schema_issuer_did_pattern(cls, value):
+    @validator("tails_hash")
+    def tails_hash_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^(did:sov:)?[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}$"
+        pattern = (
+            r"^[123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{43,44}$"
+        )
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of schema_issuer_did does not match regex pattern ('{pattern}')"
+                f"Value of tails_hash does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("schema_version")
-    def schema_version_pattern(cls, value):
+    @validator("updated_at")
+    def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
-        pattern = r"^[0-9.]+$"
+        pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
-                f"Value of schema_version does not match regex pattern ('{pattern}')"
+                f"Value of updated_at does not match regex pattern ('{pattern}')"
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V10CredentialProposalRequestMand.update_forward_refs()
+IssuerRevRegRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_credential_store_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_store_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     V10CredentialStoreRequest - a model defined in OpenAPI
         credential_id: The credential_id of this V10CredentialStoreRequest [Optional].
     """
 
     credential_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        credential_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_id=credential_id,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10CredentialStoreRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_discovery_exchange_list_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V10DiscoveryExchangeListResult - a model defined in OpenAPI
         results: The results of this V10DiscoveryExchangeListResult [Optional].
     """
 
     results: Optional[List[V10DiscoveryRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[V10DiscoveryRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10DiscoveryExchangeListResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_discovery_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_discovery_record.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,41 +35,14 @@
     discovery_exchange_id: Optional[str] = None
     query_msg: Optional[Query] = None
     state: Optional[str] = None
     thread_id: Optional[str] = None
     trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: Optional[str] = None,
-        created_at: Optional[str] = None,
-        disclose: Optional[Disclose] = None,
-        discovery_exchange_id: Optional[str] = None,
-        query_msg: Optional[Query] = None,
-        state: Optional[str] = None,
-        thread_id: Optional[str] = None,
-        trace: Optional[bool] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            connection_id=connection_id,
-            created_at=created_at,
-            disclose=disclose,
-            discovery_exchange_id=discovery_exchange_id,
-            query_msg=query_msg,
-            state=state,
-            thread_id=thread_id,
-            trace=trace,
-            updated_at=updated_at,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_create_request_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_create_request_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,29 +24,12 @@
     """
 
     proof_request: IndyProofRequest
     auto_verify: Optional[bool] = None
     comment: Optional[str] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        proof_request: IndyProofRequest = None,
-        auto_verify: Optional[bool] = None,
-        comment: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_verify=auto_verify,
-            comment=comment,
-            proof_request=proof_request,
-            trace=trace,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10PresentationCreateRequestRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_exchange_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_exchange_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,23 +20,12 @@
 
     V10PresentationExchangeList - a model defined in OpenAPI
         results: Aries RFC 37 v1.0 presentation exchange records [Optional].
     """
 
     results: Optional[List[V10PresentationExchange]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[V10PresentationExchange]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10PresentationExchangeList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_problem_report_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_problem_report_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     V10PresentationProblemReportRequest - a model defined in OpenAPI
         description: The description of this V10PresentationProblemReportRequest.
     """
 
     description: str
 
-    def __init__(
-        self,
-        *,
-        description: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            description=description,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10PresentationProblemReportRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_proposal_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_send_request_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,53 +4,34 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.indy_pres_preview import IndyPresPreview
+from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
 
 
-class V10PresentationProposalRequest(BaseModel):
+class V10PresentationSendRequestRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V10PresentationProposalRequest - a model defined in OpenAPI
+    V10PresentationSendRequestRequest - a model defined in OpenAPI
         connection_id: Connection identifier.
-        presentation_proposal: The presentation_proposal of this V10PresentationProposalRequest.
-        auto_present: Whether to respond automatically to presentation requests, building and presenting requested proof [Optional].
-        comment: Human-readable comment [Optional].
+        proof_request: The proof_request of this V10PresentationSendRequestRequest.
+        auto_verify: Verifier choice to auto-verify proof presentation [Optional].
+        comment: The comment of this V10PresentationSendRequestRequest [Optional].
         trace: Whether to trace event (default false) [Optional].
     """
 
     connection_id: str
-    presentation_proposal: IndyPresPreview
-    auto_present: Optional[bool] = None
+    proof_request: IndyProofRequest
+    auto_verify: Optional[bool] = None
     comment: Optional[str] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: str = None,
-        presentation_proposal: IndyPresPreview = None,
-        auto_present: Optional[bool] = None,
-        comment: Optional[str] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_present=auto_present,
-            comment=comment,
-            connection_id=connection_id,
-            presentation_proposal=presentation_proposal,
-            trace=trace,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
-V10PresentationProposalRequest.update_forward_refs()
+V10PresentationSendRequestRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_send_request_to_proposal.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,25 +19,12 @@
         auto_verify: Verifier choice to auto-verify proof presentation [Optional].
         trace: Whether to trace event (default false) [Optional].
     """
 
     auto_verify: Optional[bool] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        auto_verify: Optional[bool] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_verify=auto_verify,
-            trace=trace,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V10PresentationSendRequestToProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_attr_spec.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/query.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,42 +6,29 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V20CredAttrSpec(BaseModel):
+class Query(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredAttrSpec - a model defined in OpenAPI
-        name: Attribute name.
-        value: Attribute value: base64-encode if MIME type is present.
-        mime_type: MIME type: omit for (null) default [Optional].
+    Query - a model defined in OpenAPI
+        query: The query of this Query.
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        comment: The comment of this Query [Optional].
     """
 
-    name: str
-    value: str
-    mime_type: Optional[str] = Field(None, alias="mime-type")
-
-    def __init__(
-        self,
-        *,
-        name: str = None,
-        value: str = None,
-        mime_type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            mime_type=mime_type,
-            name=name,
-            value=value,
-            **kwargs,
-        )
+    query: str
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    comment: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredAttrSpec.update_forward_refs()
+Query.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_bound_offer_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_bound_offer_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,25 +21,12 @@
         counter_preview: Optional content for counter-proposal [Optional].
         filter: Credential specification criteria by format [Optional].
     """
 
     counter_preview: Optional[V20CredPreview] = None
     filter: Optional[V20CredFilter] = None
 
-    def __init__(
-        self,
-        *,
-        counter_preview: Optional[V20CredPreview] = None,
-        filter: Optional[V20CredFilter] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            counter_preview=counter_preview,
-            filter=filter,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredBoundOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_free.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_free.py`

 * *Files 22% similar despite different names*

```diff
@@ -31,35 +31,12 @@
     filter: V20CredFilter
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     trace: Optional[bool] = None
     verification_method: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: str = None,
-        filter: V20CredFilter = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        trace: Optional[bool] = None,
-        verification_method: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_remove=auto_remove,
-            comment=comment,
-            connection_id=connection_id,
-            credential_preview=credential_preview,
-            filter=filter,
-            trace=trace,
-            verification_method=verification_method,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredExFree.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_by_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,29 +23,12 @@
     """
 
     cred_issue: Optional[Dict[str, Any]] = None
     cred_offer: Optional[Dict[str, Any]] = None
     cred_proposal: Optional[Dict[str, Any]] = None
     cred_request: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        cred_issue: Optional[Dict[str, Any]] = None,
-        cred_offer: Optional[Dict[str, Any]] = None,
-        cred_proposal: Optional[Dict[str, Any]] = None,
-        cred_request: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_issue=cred_issue,
-            cred_offer=cred_offer,
-            cred_proposal=cred_proposal,
-            cred_request=cred_request,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredExRecordByFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_detail.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_detail.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,27 +26,12 @@
         ld_proof: The ld_proof of this V20CredExRecordDetail [Optional].
     """
 
     cred_ex_record: Optional[V20CredExRecord] = None
     indy: Optional[V20CredExRecordIndy] = None
     ld_proof: Optional[V20CredExRecordLDProof] = None
 
-    def __init__(
-        self,
-        *,
-        cred_ex_record: Optional[V20CredExRecord] = None,
-        indy: Optional[V20CredExRecordIndy] = None,
-        ld_proof: Optional[V20CredExRecordLDProof] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_ex_record=cred_ex_record,
-            indy=indy,
-            ld_proof=ld_proof,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredExRecordDetail.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_indy.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_presentation_exchange.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,109 +4,78 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.indy_proof import IndyProof
+from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
+from aries_cloudcontroller.model.presentation_proposal import PresentationProposal
+from aries_cloudcontroller.model.presentation_request import PresentationRequest
 
 
-class V20CredExRecordIndy(BaseModel):
+class V10PresentationExchange(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredExRecordIndy - a model defined in OpenAPI
+    V10PresentationExchange - a model defined in OpenAPI
+        auto_present: Prover choice to auto-present proof as verifier requests [Optional].
+        auto_verify: Verifier choice to auto-verify proof presentation [Optional].
+        connection_id: Connection identifier [Optional].
         created_at: Time of record creation [Optional].
-        cred_ex_id: Corresponding v2.0 credential exchange record identifier [Optional].
-        cred_ex_indy_id: Record identifier [Optional].
-        cred_id_stored: Credential identifier stored in wallet [Optional].
-        cred_request_metadata: Credential request metadata for indy holder [Optional].
-        cred_rev_id: Credential revocation identifier within revocation registry [Optional].
-        rev_reg_id: Revocation registry identifier [Optional].
-        state: Current record state [Optional].
+        error_msg: Error message [Optional].
+        initiator: Present-proof exchange initiator: self or external [Optional].
+        presentation: (Indy) presentation (also known as proof) [Optional].
+        presentation_exchange_id: Presentation exchange identifier [Optional].
+        presentation_proposal_dict: Presentation proposal message [Optional].
+        presentation_request: (Indy) presentation request (also known as proof request) [Optional].
+        presentation_request_dict: Presentation request message [Optional].
+        role: Present-proof exchange role: prover or verifier [Optional].
+        state: Present-proof exchange state [Optional].
+        thread_id: Thread identifier [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
+        verified: Whether presentation is verified: true or false [Optional].
+        verified_msgs: The verified_msgs of this V10PresentationExchange [Optional].
     """
 
+    auto_present: Optional[bool] = None
+    auto_verify: Optional[bool] = None
+    connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    cred_ex_id: Optional[str] = None
-    cred_ex_indy_id: Optional[str] = None
-    cred_id_stored: Optional[str] = None
-    cred_request_metadata: Optional[Dict[str, Any]] = None
-    cred_rev_id: Optional[str] = None
-    rev_reg_id: Optional[str] = None
+    error_msg: Optional[str] = None
+    initiator: Optional[Literal["self", "external"]] = None
+    presentation: Optional[IndyProof] = None
+    presentation_exchange_id: Optional[str] = None
+    presentation_proposal_dict: Optional[PresentationProposal] = None
+    presentation_request: Optional[IndyProofRequest] = None
+    presentation_request_dict: Optional[PresentationRequest] = None
+    role: Optional[Literal["prover", "verifier"]] = None
     state: Optional[str] = None
+    thread_id: Optional[str] = None
+    trace: Optional[bool] = None
     updated_at: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        created_at: Optional[str] = None,
-        cred_ex_id: Optional[str] = None,
-        cred_ex_indy_id: Optional[str] = None,
-        cred_id_stored: Optional[str] = None,
-        cred_request_metadata: Optional[Dict[str, Any]] = None,
-        cred_rev_id: Optional[str] = None,
-        rev_reg_id: Optional[str] = None,
-        state: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            cred_ex_id=cred_ex_id,
-            cred_ex_indy_id=cred_ex_indy_id,
-            cred_id_stored=cred_id_stored,
-            cred_request_metadata=cred_request_metadata,
-            cred_rev_id=cred_rev_id,
-            rev_reg_id=rev_reg_id,
-            state=state,
-            updated_at=updated_at,
-            **kwargs,
-        )
+    verified: Optional[Literal["true", "false"]] = None
+    verified_msgs: Optional[List[str]] = None
 
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
         if not re.match(pattern, value):
             raise ValueError(
                 f"Value of created_at does not match regex pattern ('{pattern}')"
             )
         return value
 
-    @validator("cred_rev_id")
-    def cred_rev_id_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^[1-9][0-9]*$"
-        if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of cred_rev_id does not match regex pattern ('{pattern}')"
-            )
-        return value
-
-    @validator("rev_reg_id")
-    def rev_reg_id_pattern(cls, value):
-        # Property is optional
-        if value is None:
-            return
-
-        pattern = r"^([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):4:([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}):3:CL:(([1-9][0-9]*)|([123456789ABCDEFGHJKLMNPQRSTUVWXYZabcdefghijkmnopqrstuvwxyz]{21,22}:2:.+:[0-9.]+))(:.+)?:CL_ACCUM:(.+$)"
-        if not re.match(pattern, value):
-            raise ValueError(
-                f"Value of rev_reg_id does not match regex pattern ('{pattern}')"
-            )
-        return value
-
     @validator("updated_at")
     def updated_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
@@ -116,8 +85,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredExRecordIndy.update_forward_refs()
+V10PresentationExchange.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_ex_record_list_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V20CredExRecordListResult - a model defined in OpenAPI
         results: Credential exchange records and corresponding detail records [Optional].
     """
 
     results: Optional[List[V20CredExRecordDetail]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[V20CredExRecordDetail]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredExRecordListResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,42 +4,37 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.ld_proof_vc_detail import LDProofVCDetail
-from aries_cloudcontroller.model.v20_cred_filter_indy import V20CredFilterIndy
+from aries_cloudcontroller.model.attach_decorator import AttachDecorator
+from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
 
 
-class V20CredFilter(BaseModel):
+class V20CredIssue(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredFilter - a model defined in OpenAPI
-        indy: Credential filter for indy [Optional].
-        ld_proof: Credential filter for linked data proof [Optional].
+    V20CredIssue - a model defined in OpenAPI
+        credentialsattach: Credential attachments.
+        formats: Acceptable attachment formats.
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        comment: Human-readable comment [Optional].
+        replacement_id: Issuer-unique identifier to coordinate credential replacement [Optional].
     """
 
-    indy: Optional[V20CredFilterIndy] = None
-    ld_proof: Optional[LDProofVCDetail] = None
-
-    def __init__(
-        self,
-        *,
-        indy: Optional[V20CredFilterIndy] = None,
-        ld_proof: Optional[LDProofVCDetail] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            indy=indy,
-            ld_proof=ld_proof,
-            **kwargs,
-        )
+    credentialsattach: List[AttachDecorator] = Field(..., alias="credentials~attach")
+    formats: List[V20CredFormat]
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    comment: Optional[str] = None
+    replacement_id: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredFilter.update_forward_refs()
+V20CredIssue.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter_indy.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v10_credential_proposal_request_mand.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,57 +4,47 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.credential_preview import CredentialPreview
 
 
-class V20CredFilterIndy(BaseModel):
+class V10CredentialProposalRequestMand(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredFilterIndy - a model defined in OpenAPI
+    V10CredentialProposalRequestMand - a model defined in OpenAPI
+        connection_id: Connection identifier.
+        credential_proposal: The credential_proposal of this V10CredentialProposalRequestMand.
+        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
+        comment: Human-readable comment [Optional].
         cred_def_id: Credential definition identifier [Optional].
         issuer_did: Credential issuer DID [Optional].
         schema_id: Schema identifier [Optional].
         schema_issuer_did: Schema issuer DID [Optional].
         schema_name: Schema name [Optional].
         schema_version: Schema version [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
     """
 
+    connection_id: str
+    credential_proposal: CredentialPreview
+    auto_remove: Optional[bool] = None
+    comment: Optional[str] = None
     cred_def_id: Optional[str] = None
     issuer_did: Optional[str] = None
     schema_id: Optional[str] = None
     schema_issuer_did: Optional[str] = None
     schema_name: Optional[str] = None
     schema_version: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        cred_def_id: Optional[str] = None,
-        issuer_did: Optional[str] = None,
-        schema_id: Optional[str] = None,
-        schema_issuer_did: Optional[str] = None,
-        schema_name: Optional[str] = None,
-        schema_version: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            cred_def_id=cred_def_id,
-            issuer_did=issuer_did,
-            schema_id=schema_id,
-            schema_issuer_did=schema_issuer_did,
-            schema_name=schema_name,
-            schema_version=schema_version,
-            **kwargs,
-        )
+    trace: Optional[bool] = None
 
     @validator("cred_def_id")
     def cred_def_id_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
@@ -117,8 +107,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredFilterIndy.update_forward_refs()
+V10CredentialProposalRequestMand.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/send_message.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,37 +4,25 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.ld_proof_vc_detail import LDProofVCDetail
 
 
-class V20CredFilterLDProof(BaseModel):
+class SendMessage(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredFilterLDProof - a model defined in OpenAPI
-        ld_proof: Credential filter for linked data proof.
+    SendMessage - a model defined in OpenAPI
+        content: Message content [Optional].
     """
 
-    ld_proof: LDProofVCDetail
-
-    def __init__(
-        self,
-        *,
-        ld_proof: LDProofVCDetail = None,
-        **kwargs,
-    ):
-        super().__init__(
-            ld_proof=ld_proof,
-            **kwargs,
-        )
+    content: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredFilterLDProof.update_forward_refs()
+SendMessage.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,40 +4,35 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.attach_decorator import AttachDecorator
+from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
 
 
-class V20CredFormat(BaseModel):
+class V20CredRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredFormat - a model defined in OpenAPI
-        attach_id: Attachment identifier.
-        format: Attachment format specifier.
+    V20CredRequest - a model defined in OpenAPI
+        formats: Acceptable attachment formats.
+        requestsattach: Request attachments.
+        id: Message identifier [Optional].
+        type: Message type [Optional].
+        comment: Human-readable comment [Optional].
     """
 
-    attach_id: str
-    format: str
-
-    def __init__(
-        self,
-        *,
-        attach_id: str = None,
-        format: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            attach_id=attach_id,
-            format=format,
-            **kwargs,
-        )
+    formats: List[V20CredFormat]
+    requestsattach: List[AttachDecorator] = Field(..., alias="requests~attach")
+    id: Optional[str] = Field(None, alias="@id")
+    type: Optional[str] = Field(None, alias="@type")
+    comment: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredFormat.update_forward_refs()
+V20CredRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,58 +4,39 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attach_decorator import AttachDecorator
-from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
+from aries_cloudcontroller.model.v20_cred_filter import V20CredFilter
+from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
 
 
-class V20CredIssue(BaseModel):
+class V20CredOfferRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredIssue - a model defined in OpenAPI
-        credentialsattach: Credential attachments.
-        formats: Acceptable attachment formats.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
+    V20CredOfferRequest - a model defined in OpenAPI
+        connection_id: Connection identifier.
+        filter: Credential specification criteria by format.
+        auto_issue: Whether to respond automatically to credential requests, creating and issuing requested credentials [Optional].
+        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
-        replacement_id: Issuer-unique identifier to coordinate credential replacement [Optional].
+        credential_preview: The credential_preview of this V20CredOfferRequest [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
     """
 
-    credentialsattach: List[AttachDecorator] = Field(..., alias="credentials~attach")
-    formats: List[V20CredFormat]
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
+    connection_id: str
+    filter: V20CredFilter
+    auto_issue: Optional[bool] = None
+    auto_remove: Optional[bool] = None
     comment: Optional[str] = None
-    replacement_id: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        credentialsattach: List[AttachDecorator] = None,
-        formats: List[V20CredFormat] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        replacement_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            credentialsattach=credentialsattach,
-            formats=formats,
-            replacement_id=replacement_id,
-            **kwargs,
-        )
+    credential_preview: Optional[V20CredPreview] = None
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredIssue.update_forward_refs()
+V20CredOfferRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_filter_ld_proof.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,36 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.ld_proof_vc_detail import LDProofVCDetail
 
 
-class V20CredIssueProblemReportRequest(BaseModel):
+class V20CredFilterLDProof(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredIssueProblemReportRequest - a model defined in OpenAPI
-        description: The description of this V20CredIssueProblemReportRequest.
+    V20CredFilterLDProof - a model defined in OpenAPI
+        ld_proof: Credential filter for linked data proof.
     """
 
-    description: str
-
-    def __init__(
-        self,
-        *,
-        description: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            description=description,
-            **kwargs,
-        )
+    ld_proof: LDProofVCDetail
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredIssueProblemReportRequest.update_forward_refs()
+V20CredFilterLDProof.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_issue_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_request_free.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,36 +4,36 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.v20_cred_filter_ld_proof import V20CredFilterLDProof
 
 
-class V20CredIssueRequest(BaseModel):
+class V20CredRequestFree(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredIssueRequest - a model defined in OpenAPI
+    V20CredRequestFree - a model defined in OpenAPI
+        connection_id: Connection identifier.
+        filter: Credential specification criteria by format.
+        auto_remove: Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting) [Optional].
         comment: Human-readable comment [Optional].
+        holder_did: Holder DID to substitute for the credentialSubject.id [Optional].
+        trace: Whether to trace event (default false) [Optional].
     """
 
+    connection_id: str
+    filter: V20CredFilterLDProof
+    auto_remove: Optional[bool] = None
     comment: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            comment=comment,
-            **kwargs,
-        )
+    holder_did: Optional[str] = None
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredIssueRequest.update_forward_refs()
+V20CredRequestFree.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_offer.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,35 +32,12 @@
     offersattach: List[AttachDecorator] = Field(..., alias="offers~attach")
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     replacement_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        formats: List[V20CredFormat] = None,
-        offersattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        replacement_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            credential_preview=credential_preview,
-            formats=formats,
-            offersattach=offersattach,
-            replacement_id=replacement_id,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredOffer.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_offer_conn_free_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,33 +29,12 @@
     filter: V20CredFilter
     auto_issue: Optional[bool] = None
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        filter: V20CredFilter = None,
-        auto_issue: Optional[bool] = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_issue=auto_issue,
-            auto_remove=auto_remove,
-            comment=comment,
-            credential_preview=credential_preview,
-            filter=filter,
-            trace=trace,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredOfferConnFreeRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_preview.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_presentation_send_request_to_proposal.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,41 +4,27 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.v20_cred_attr_spec import V20CredAttrSpec
 
 
-class V20CredPreview(BaseModel):
+class V20PresentationSendRequestToProposal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredPreview - a model defined in OpenAPI
-        attributes: The attributes of this V20CredPreview.
-        type: Message type identifier [Optional].
+    V20PresentationSendRequestToProposal - a model defined in OpenAPI
+        auto_verify: Verifier choice to auto-verify proof presentation [Optional].
+        trace: Whether to trace event (default false) [Optional].
     """
 
-    attributes: List[V20CredAttrSpec]
-    type: Optional[str] = Field(None, alias="@type")
-
-    def __init__(
-        self,
-        *,
-        attributes: List[V20CredAttrSpec] = None,
-        type: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            type=type,
-            attributes=attributes,
-            **kwargs,
-        )
+    auto_verify: Optional[bool] = None
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredPreview.update_forward_refs()
+V20PresentationSendRequestToProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/input_descriptors.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,59 +4,41 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.attach_decorator import AttachDecorator
-from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
-from aries_cloudcontroller.model.v20_cred_preview import V20CredPreview
+from aries_cloudcontroller.model.constraints import Constraints
+from aries_cloudcontroller.model.schemas_input_descriptor_filter import (
+    SchemasInputDescriptorFilter,
+)
 
 
-class V20CredProposal(BaseModel):
+class InputDescriptors(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredProposal - a model defined in OpenAPI
-        filtersattach: Credential filter per acceptable format on corresponding identifier.
-        formats: Attachment formats.
-        id: Message identifier [Optional].
-        type: Message type [Optional].
-        comment: Human-readable comment [Optional].
-        credential_preview: Credential preview [Optional].
+    InputDescriptors - a model defined in OpenAPI
+        constraints: The constraints of this InputDescriptors [Optional].
+        group: The group of this InputDescriptors [Optional].
+        id: ID [Optional].
+        metadata: Metadata dictionary [Optional].
+        name: Name [Optional].
+        purpose: Purpose [Optional].
+        schema_: Accepts a list of schema or a dict containing filters like oneof_filter. [Optional].
     """
 
-    filtersattach: List[AttachDecorator] = Field(..., alias="filters~attach")
-    formats: List[V20CredFormat]
-    id: Optional[str] = Field(None, alias="@id")
-    type: Optional[str] = Field(None, alias="@type")
-    comment: Optional[str] = None
-    credential_preview: Optional[V20CredPreview] = None
-
-    def __init__(
-        self,
-        *,
-        filtersattach: List[AttachDecorator] = None,
-        formats: List[V20CredFormat] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            credential_preview=credential_preview,
-            filtersattach=filtersattach,
-            formats=formats,
-            **kwargs,
-        )
+    constraints: Optional[Constraints] = None
+    group: Optional[List[str]] = None
+    id: Optional[str] = None
+    metadata: Optional[Dict[str, Any]] = None
+    name: Optional[str] = None
+    purpose: Optional[str] = None
+    schema_: Optional[SchemasInputDescriptorFilter] = Field(None, alias="schema")
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredProposal.update_forward_refs()
+InputDescriptors.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_proposal.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,53 +5,34 @@
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
-from aries_cloudcontroller.model.v20_cred_format import V20CredFormat
+from aries_cloudcontroller.model.v20_pres_format import V20PresFormat
 
 
-class V20CredRequest(BaseModel):
+class V20PresProposal(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredRequest - a model defined in OpenAPI
-        formats: Acceptable attachment formats.
-        requestsattach: Request attachments.
+    V20PresProposal - a model defined in OpenAPI
+        formats: The formats of this V20PresProposal.
+        proposalsattach: Attachment per acceptable format on corresponding identifier.
         id: Message identifier [Optional].
         type: Message type [Optional].
         comment: Human-readable comment [Optional].
     """
 
-    formats: List[V20CredFormat]
-    requestsattach: List[AttachDecorator] = Field(..., alias="requests~attach")
+    formats: List[V20PresFormat]
+    proposalsattach: List[AttachDecorator] = Field(..., alias="proposals~attach")
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        formats: List[V20CredFormat] = None,
-        requestsattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            formats=formats,
-            requestsattach=requestsattach,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredRequest.update_forward_refs()
+V20PresProposal.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_request_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/publish_revocations.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V20CredRequestRequest(BaseModel):
+class PublishRevocations(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20CredRequestRequest - a model defined in OpenAPI
-        holder_did: Holder DID to substitute for the credentialSubject.id [Optional].
+    PublishRevocations - a model defined in OpenAPI
+        rrid2crid: Credential revocation ids by revocation registry id [Optional].
     """
 
-    holder_did: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        holder_did: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            holder_did=holder_did,
-            **kwargs,
-        )
+    rrid2crid: Optional[Dict[str, List[str]]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20CredRequestRequest.update_forward_refs()
+PublishRevocations.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_cred_store_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_store_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,23 +17,12 @@
 
     V20CredStoreRequest - a model defined in OpenAPI
         credential_id: The credential_id of this V20CredStoreRequest [Optional].
     """
 
     credential_id: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        credential_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            credential_id=credential_id,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20CredStoreRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_discovery_exchange_result.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_discovery_exchange_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V20DiscoveryExchangeResult - a model defined in OpenAPI
         results: Discover Features v2.0 exchange record [Optional].
     """
 
     results: Optional[V20DiscoveryRecord] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[V20DiscoveryRecord] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20DiscoveryExchangeResult.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_discovery_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/invitation_record.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,72 +4,44 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.disclosures import Disclosures
-from aries_cloudcontroller.model.queries import Queries
+from aries_cloudcontroller.model.invitation_message import InvitationMessage
 
 
-class V20DiscoveryRecord(BaseModel):
+class InvitationRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20DiscoveryRecord - a model defined in OpenAPI
-        connection_id: Connection identifier [Optional].
+    InvitationRecord - a model defined in OpenAPI
         created_at: Time of record creation [Optional].
-        disclosures: Disclosures message [Optional].
-        discovery_exchange_id: Credential exchange identifier [Optional].
-        queries_msg: Queries message [Optional].
-        state: Current record state [Optional].
-        thread_id: Thread identifier [Optional].
+        invi_msg_id: Invitation message identifier [Optional].
+        invitation: Out of band invitation message [Optional].
+        invitation_id: Invitation record identifier [Optional].
+        invitation_url: Invitation message URL [Optional].
+        oob_id: Out of band record identifier [Optional].
+        state: Out of band message exchange state [Optional].
         trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
     """
 
-    connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    disclosures: Optional[Disclosures] = None
-    discovery_exchange_id: Optional[str] = None
-    queries_msg: Optional[Queries] = None
+    invi_msg_id: Optional[str] = None
+    invitation: Optional[InvitationMessage] = None
+    invitation_id: Optional[str] = None
+    invitation_url: Optional[str] = None
+    oob_id: Optional[str] = None
     state: Optional[str] = None
-    thread_id: Optional[str] = None
     trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        connection_id: Optional[str] = None,
-        created_at: Optional[str] = None,
-        disclosures: Optional[Disclosures] = None,
-        discovery_exchange_id: Optional[str] = None,
-        queries_msg: Optional[Queries] = None,
-        state: Optional[str] = None,
-        thread_id: Optional[str] = None,
-        trace: Optional[bool] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            connection_id=connection_id,
-            created_at=created_at,
-            disclosures=disclosures,
-            discovery_exchange_id=discovery_exchange_id,
-            queries_msg=queries_msg,
-            state=state,
-            thread_id=thread_id,
-            trace=trace,
-            updated_at=updated_at,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
@@ -92,8 +64,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20DiscoveryRecord.update_forward_refs()
+InvitationRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_issue_cred_schema_core.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_issue_cred_schema_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,31 +27,12 @@
 
     filter: V20CredFilter
     auto_remove: Optional[bool] = None
     comment: Optional[str] = None
     credential_preview: Optional[V20CredPreview] = None
     trace: Optional[bool] = None
 
-    def __init__(
-        self,
-        *,
-        filter: V20CredFilter = None,
-        auto_remove: Optional[bool] = None,
-        comment: Optional[str] = None,
-        credential_preview: Optional[V20CredPreview] = None,
-        trace: Optional[bool] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            auto_remove=auto_remove,
-            comment=comment,
-            credential_preview=credential_preview,
-            filter=filter,
-            trace=trace,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20IssueCredSchemaCore.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,31 +29,12 @@
     presentationsattach: List[AttachDecorator] = Field(
         ..., alias="presentations~attach"
     )
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        formats: List[V20PresFormat] = None,
-        presentationsattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            formats=formats,
-            presentationsattach=presentationsattach,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20Pres.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_ex_record_by_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,27 +21,12 @@
         pres_request: The pres_request of this V20PresExRecordByFormat [Optional].
     """
 
     pres: Optional[Dict[str, Any]] = None
     pres_proposal: Optional[Dict[str, Any]] = None
     pres_request: Optional[Dict[str, Any]] = None
 
-    def __init__(
-        self,
-        *,
-        pres: Optional[Dict[str, Any]] = None,
-        pres_proposal: Optional[Dict[str, Any]] = None,
-        pres_request: Optional[Dict[str, Any]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            pres=pres,
-            pres_proposal=pres_proposal,
-            pres_request=pres_request,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20PresExRecordByFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_ex_record_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_ex_record_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,23 +18,12 @@
 
     V20PresExRecordList - a model defined in OpenAPI
         results: Presentation exchange records [Optional].
     """
 
     results: Optional[List[V20PresExRecord]] = None
 
-    def __init__(
-        self,
-        *,
-        results: Optional[List[V20PresExRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 V20PresExRecordList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_problem_report_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_cred_issue_problem_report_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class V20PresProblemReportRequest(BaseModel):
+class V20CredIssueProblemReportRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresProblemReportRequest - a model defined in OpenAPI
-        description: The description of this V20PresProblemReportRequest.
+    V20CredIssueProblemReportRequest - a model defined in OpenAPI
+        description: The description of this V20CredIssueProblemReportRequest.
     """
 
     description: str
 
-    def __init__(
-        self,
-        *,
-        description: str = None,
-        **kwargs,
-    ):
-        super().__init__(
-            description=description,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresProblemReportRequest.update_forward_refs()
+V20CredIssueProblemReportRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_proposal.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,50 +8,35 @@
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 from aries_cloudcontroller.model.attach_decorator import AttachDecorator
 from aries_cloudcontroller.model.v20_pres_format import V20PresFormat
 
 
-class V20PresProposal(BaseModel):
+class V20PresRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresProposal - a model defined in OpenAPI
-        formats: The formats of this V20PresProposal.
-        proposalsattach: Attachment per acceptable format on corresponding identifier.
+    V20PresRequest - a model defined in OpenAPI
+        formats: The formats of this V20PresRequest.
+        request_presentationsattach: Attachment per acceptable format on corresponding identifier.
         id: Message identifier [Optional].
         type: Message type [Optional].
         comment: Human-readable comment [Optional].
+        will_confirm: Whether verifier will send confirmation ack [Optional].
     """
 
     formats: List[V20PresFormat]
-    proposalsattach: List[AttachDecorator] = Field(..., alias="proposals~attach")
+    request_presentationsattach: List[AttachDecorator] = Field(
+        ..., alias="request_presentations~attach"
+    )
     id: Optional[str] = Field(None, alias="@id")
     type: Optional[str] = Field(None, alias="@type")
     comment: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        formats: List[V20PresFormat] = None,
-        proposalsattach: List[AttachDecorator] = None,
-        id: Optional[str] = None,
-        type: Optional[str] = None,
-        comment: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            id=id,
-            type=type,
-            comment=comment,
-            formats=formats,
-            proposalsattach=proposalsattach,
-            **kwargs,
-        )
+    will_confirm: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresProposal.update_forward_refs()
+V20PresRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_proposal_by_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_request_by_format.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,42 +4,29 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.dif_proof_proposal import DIFProofProposal
+from aries_cloudcontroller.model.dif_proof_request import DIFProofRequest
 from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
 
 
-class V20PresProposalByFormat(BaseModel):
+class V20PresRequestByFormat(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresProposalByFormat - a model defined in OpenAPI
-        dif: Presentation proposal for DIF [Optional].
-        indy: Presentation proposal for indy [Optional].
+    V20PresRequestByFormat - a model defined in OpenAPI
+        dif: Presentation request for DIF [Optional].
+        indy: Presentation request for indy [Optional].
     """
 
-    dif: Optional[DIFProofProposal] = None
+    dif: Optional[DIFProofRequest] = None
     indy: Optional[IndyProofRequest] = None
 
-    def __init__(
-        self,
-        *,
-        dif: Optional[DIFProofProposal] = None,
-        indy: Optional[IndyProofRequest] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            dif=dif,
-            indy=indy,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresProposalByFormat.update_forward_refs()
+V20PresRequestByFormat.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/v20_pres_request_by_format.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/v20_pres_spec_by_format_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,42 +4,31 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.dif_proof_request import DIFProofRequest
-from aries_cloudcontroller.model.indy_proof_request import IndyProofRequest
+from aries_cloudcontroller.model.dif_pres_spec import DIFPresSpec
+from aries_cloudcontroller.model.indy_pres_spec import IndyPresSpec
 
 
-class V20PresRequestByFormat(BaseModel):
+class V20PresSpecByFormatRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    V20PresRequestByFormat - a model defined in OpenAPI
-        dif: Presentation request for DIF [Optional].
-        indy: Presentation request for indy [Optional].
+    V20PresSpecByFormatRequest - a model defined in OpenAPI
+        dif: Optional Presentation specification for DIF, overrides the PresentionExchange record&#39;s PresRequest [Optional].
+        indy: Presentation specification for indy [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
     """
 
-    dif: Optional[DIFProofRequest] = None
-    indy: Optional[IndyProofRequest] = None
-
-    def __init__(
-        self,
-        *,
-        dif: Optional[DIFProofRequest] = None,
-        indy: Optional[IndyProofRequest] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            dif=dif,
-            indy=indy,
-            **kwargs,
-        )
+    dif: Optional[DIFPresSpec] = None
+    indy: Optional[IndyPresSpec] = None
+    trace: Optional[bool] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-V20PresRequestByFormat.update_forward_refs()
+V20PresSpecByFormatRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/vc_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/w3_c_credentials_list_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,70 +6,39 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class VCRecord(BaseModel):
+class W3CCredentialsListRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    VCRecord - a model defined in OpenAPI
-        contexts: The contexts of this VCRecord [Optional].
-        cred_tags: The cred_tags of this VCRecord [Optional].
-        cred_value: (JSON-serializable) credential value [Optional].
-        expanded_types: The expanded_types of this VCRecord [Optional].
-        given_id: Credential identifier [Optional].
-        issuer_id: Issuer identifier [Optional].
-        proof_types: The proof_types of this VCRecord [Optional].
-        record_id: Record identifier [Optional].
-        schema_ids: The schema_ids of this VCRecord [Optional].
-        subject_ids: The subject_ids of this VCRecord [Optional].
+    W3CCredentialsListRequest - a model defined in OpenAPI
+        contexts: The contexts of this W3CCredentialsListRequest [Optional].
+        given_id: Given credential id to match [Optional].
+        issuer_id: Credential issuer identifier to match [Optional].
+        max_results: Maximum number of results to return [Optional].
+        proof_types: The proof_types of this W3CCredentialsListRequest [Optional].
+        schema_ids: Schema identifiers, all of which to match [Optional].
+        subject_ids: Subject identifiers, all of which to match [Optional].
+        tag_query: Tag filter [Optional].
+        types: The types of this W3CCredentialsListRequest [Optional].
     """
 
     contexts: Optional[List[str]] = None
-    cred_tags: Optional[Dict[str, str]] = None
-    cred_value: Optional[Dict[str, Any]] = None
-    expanded_types: Optional[List[str]] = None
     given_id: Optional[str] = None
     issuer_id: Optional[str] = None
+    max_results: Optional[int] = None
     proof_types: Optional[List[str]] = None
-    record_id: Optional[str] = None
     schema_ids: Optional[List[str]] = None
     subject_ids: Optional[List[str]] = None
-
-    def __init__(
-        self,
-        *,
-        contexts: Optional[List[str]] = None,
-        cred_tags: Optional[Dict[str, str]] = None,
-        cred_value: Optional[Dict[str, Any]] = None,
-        expanded_types: Optional[List[str]] = None,
-        given_id: Optional[str] = None,
-        issuer_id: Optional[str] = None,
-        proof_types: Optional[List[str]] = None,
-        record_id: Optional[str] = None,
-        schema_ids: Optional[List[str]] = None,
-        subject_ids: Optional[List[str]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            contexts=contexts,
-            cred_tags=cred_tags,
-            cred_value=cred_value,
-            expanded_types=expanded_types,
-            given_id=given_id,
-            issuer_id=issuer_id,
-            proof_types=proof_types,
-            record_id=record_id,
-            schema_ids=schema_ids,
-            subject_ids=subject_ids,
-            **kwargs,
-        )
+    tag_query: Optional[Dict[str, str]] = None
+    types: Optional[List[str]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-VCRecord.update_forward_refs()
+W3CCredentialsListRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/vc_record_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/ledger_config_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,26 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.vc_record import VCRecord
+from aries_cloudcontroller.model.ledger_config_instance import LedgerConfigInstance
 
 
-class VCRecordList(BaseModel):
+class LedgerConfigList(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    VCRecordList - a model defined in OpenAPI
-        results: The results of this VCRecordList [Optional].
+    LedgerConfigList - a model defined in OpenAPI
+        ledger_config_list: The ledger_config_list of this LedgerConfigList.
     """
 
-    results: Optional[List[VCRecord]] = None
-
-    def __init__(
-        self,
-        *,
-        results: Optional[List[VCRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
+    ledger_config_list: List[LedgerConfigInstance]
 
     class Config:
         allow_population_by_field_name = True
 
 
-VCRecordList.update_forward_refs()
+LedgerConfigList.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/verify_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/verify_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,12 @@
         doc: Signed document.
         verkey: Verkey to use for doc verification [Optional].
     """
 
     doc: SignedDoc
     verkey: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        doc: SignedDoc = None,
-        verkey: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            doc=doc,
-            verkey=verkey,
-            **kwargs,
-        )
-
     class Config:
         allow_population_by_field_name = True
 
 
 VerifyRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/wallet_list.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/indy_proof_requested_proof_revealed_attr_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,28 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
-from aries_cloudcontroller.model.wallet_record import WalletRecord
+from aries_cloudcontroller.model.raw_encoded import RawEncoded
 
 
-class WalletList(BaseModel):
+class IndyProofRequestedProofRevealedAttrGroup(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    WalletList - a model defined in OpenAPI
-        results: List of wallet records [Optional].
+    IndyProofRequestedProofRevealedAttrGroup - a model defined in OpenAPI
+        sub_proof_index: Sub-proof index [Optional].
+        values: Indy proof requested proof revealed attr groups group value [Optional].
     """
 
-    results: Optional[List[WalletRecord]] = None
-
-    def __init__(
-        self,
-        *,
-        results: Optional[List[WalletRecord]] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            results=results,
-            **kwargs,
-        )
+    sub_proof_index: Optional[int] = None
+    values: Optional[Dict[str, RawEncoded]] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-WalletList.update_forward_refs()
+IndyProofRequestedProofRevealedAttrGroup.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/wallet_record.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/oob_record.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,58 +4,59 @@
 
 from datetime import date, datetime  # noqa: F401
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
+from aries_cloudcontroller.model.invitation_message import InvitationMessage
+from aries_cloudcontroller.model.service_decorator import ServiceDecorator
 
 
-class WalletRecord(BaseModel):
+class OobRecord(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    WalletRecord - a model defined in OpenAPI
-        key_management_mode: Mode regarding management of wallet key.
-        wallet_id: Wallet record ID.
+    OobRecord - a model defined in OpenAPI
+        invi_msg_id: Invitation message identifier.
+        invitation: Out of band invitation message.
+        oob_id: Oob record identifier.
+        state: Out of band message exchange state.
+        attach_thread_id: Connection record identifier [Optional].
+        connection_id: Connection record identifier [Optional].
         created_at: Time of record creation [Optional].
-        settings: Settings for this wallet. [Optional].
-        state: Current record state [Optional].
+        our_recipient_key: Recipient key used for oob invitation [Optional].
+        role: OOB Role [Optional].
+        their_service: The their_service of this OobRecord [Optional].
+        trace: Record trace information, based on agent configuration [Optional].
         updated_at: Time of last record update [Optional].
     """
 
-    key_management_mode: Literal["managed", "unmanaged"]
-    wallet_id: str
+    invi_msg_id: str
+    invitation: InvitationMessage
+    oob_id: str
+    state: Literal[
+        "initial",
+        "prepare-response",
+        "await-response",
+        "reuse-not-accepted",
+        "reuse-accepted",
+        "done",
+        "deleted",
+    ]
+    attach_thread_id: Optional[str] = None
+    connection_id: Optional[str] = None
     created_at: Optional[str] = None
-    settings: Optional[Dict[str, Any]] = None
-    state: Optional[str] = None
+    our_recipient_key: Optional[str] = None
+    role: Optional[Literal["sender", "receiver"]] = None
+    their_service: Optional[ServiceDecorator] = None
+    trace: Optional[bool] = None
     updated_at: Optional[str] = None
 
-    def __init__(
-        self,
-        *,
-        key_management_mode: Literal["managed", "unmanaged"] = None,
-        wallet_id: str = None,
-        created_at: Optional[str] = None,
-        settings: Optional[Dict[str, Any]] = None,
-        state: Optional[str] = None,
-        updated_at: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            created_at=created_at,
-            key_management_mode=key_management_mode,
-            settings=settings,
-            state=state,
-            updated_at=updated_at,
-            wallet_id=wallet_id,
-            **kwargs,
-        )
-
     @validator("created_at")
     def created_at_pattern(cls, value):
         # Property is optional
         if value is None:
             return
 
         pattern = r"^\d{4}-\d\d-\d\d[T ]\d\d:\d\d(?:\:(?:\d\d(?:\.\d{1,6})?))?(?:[+-]\d\d:?\d\d|Z|)$"
@@ -78,8 +79,8 @@
             )
         return value
 
     class Config:
         allow_population_by_field_name = True
 
 
-WalletRecord.update_forward_refs()
+OobRecord.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/model/write_ledger_request.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/model/remove_wallet_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,34 +6,23 @@
 
 import re  # noqa: F401
 from typing import Any, Dict, List, Optional, Union, Literal  # noqa: F401
 
 from pydantic import AnyUrl, BaseModel, EmailStr, validator, Field, Extra  # noqa: F401
 
 
-class WriteLedgerRequest(BaseModel):
+class RemoveWalletRequest(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator (https://openapi-generator.tech).
 
     Do not edit the class manually.
 
-    WriteLedgerRequest - a model defined in OpenAPI
-        ledger_id: The ledger_id of this WriteLedgerRequest [Optional].
+    RemoveWalletRequest - a model defined in OpenAPI
+        wallet_key: Master key used for key derivation. Only required for             unmanaged wallets. [Optional].
     """
 
-    ledger_id: Optional[str] = None
-
-    def __init__(
-        self,
-        *,
-        ledger_id: Optional[str] = None,
-        **kwargs,
-    ):
-        super().__init__(
-            ledger_id=ledger_id,
-            **kwargs,
-        )
+    wallet_key: Optional[str] = None
 
     class Config:
         allow_population_by_field_name = True
 
 
-WriteLedgerRequest.update_forward_refs()
+RemoveWalletRequest.update_forward_refs()
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller/util/pydantic_converter.py` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller/util/pydantic_converter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/PKG-INFO` & `aries_cloudcontroller-0.8.1rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aries-cloudcontroller
-Version: 0.8.0rc9
+Name: aries_cloudcontroller
+Version: 0.8.1rc4
 Summary: A simple python package for controlling an aries agent through the admin-api interface
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -55,21 +55,22 @@
 
 | Aries Cloud Controller Version | Aries Cloud Agent Python Version |
 | ------------------------------ | -------------------------------- |
 | 0.5.1-0.5.2                    | 0.7.3                            |
 | 0.6.0-0.6.3                    | 0.7.4                            |
 | 0.7.0                          | 0.7.5                            |
 | 0.8.0                          | 0.8.0                            |
+| 0.8.1                          | 0.8.1                            |
 
 ## Features
 
 Aries Cloud Controller Python is a fully featured client for interacting with ACA-Py.
 
 - Fully Typed wrapper around Aries Cloud Agent Python
-- Supports latest ACA-Py version (0.8.0)
+- Supports latest ACA-Py version (0.8.1)
 - Client is auto generated based on OpenAPI definitions, allowing us to keep up to date with new releases.
 - Supports multi-tenant APIs and authentication
 - Async API
 
 ## Usage
 
 Aries Cloud Controller Python is published to PyPi and can be installed using pip:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.8.0rc9 Summary: A
+Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.8.1rc4 Summary: A
 simple python package for controlling an aries agent through the admin-api
 interface Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python/
 tree/main/aries_cloudcontroller Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE
 
@@ -17,43 +17,44 @@
 definition provided by ACA-Py, giving a fully-typed rich API for interacting
 the cloud agent. Each Cloud Controller version maps to a specific ACA-Py
 version, which is outlined in the table below. Although not strictly adhered to
 in the past, a new ACA-Py version will result in a new Minor version bump for
 the Cloud Controller, as there are often times breaking changes. | Aries Cloud
 Controller Version | Aries Cloud Agent Python Version | | ---------------------
 --------- | -------------------------------- | | 0.5.1-0.5.2 | 0.7.3 | | 0.6.0-
-0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | ## Features Aries Cloud
-Controller Python is a fully featured client for interacting with ACA-Py. -
-Fully Typed wrapper around Aries Cloud Agent Python - Supports latest ACA-Py
-version (0.8.0) - Client is auto generated based on OpenAPI definitions,
-allowing us to keep up to date with new releases. - Supports multi-tenant APIs
-and authentication - Async API ## Usage Aries Cloud Controller Python is
-published to PyPi and can be installed using pip: ```sh pip install aries-
-cloudcontroller ``` ### Creating a client ```python from aries_cloudcontroller
-import AcaPyClient client = AcaPyClient( base_url="http://localhost:8000",
-api_key="myApiKey" ) ``` **Admin insecure mode** If you are running ACA-Py with
-the admin insecure flag and don't have the API key, you must set the
-`admin_insecure` property: ```python client = AcaPyClient( base_url="http://
-localhost:8000", # Explicitly mark that no api key is used admin_insecure=True
-) ``` **Multitenancy** To provision the agent in the context of specific tenant
-of the agent, the `tenant_jwt` property must be set: ```python client =
-AcaPyClient( base_url="http://localhost:8000", tenant_jwt="eyXXX" ) ``` ###
-Interacting with the client Once you have the client set up, you're ready to
-interact with it. Because the API is fully typed, the best way to know what is
-available is by looking at the ACA-Py swagger UI, and the available properties
-on the client. For example to create and receive an invitation the following
-methods can be called: ```python invitation = await
-client.connection.create_invitation( body=CreateInvitationRequest
-(my_label="Cloud Controller") ) connection = await
-client.connection.receive_invitation(body=result.invitation) ``` ## Available
-APIs Currently the following top-level APIs are available in the client. Each
-api maps to the topics as used by the ACA-Py swagger UI. - `action_menu` -
-`basicmessage` - `connection` - `credential_definition` - `credentials` -
-`default` - `did_exchange` - `discover_features` - `discover_features_v2_0` -
-`endorse_transaction` - `introduction` - `issue_credential_v1_0` -
-`issue_credential_v2_0` - `jsonld` - `ledger` - `mediation` - `multitenancy` -
-`out_of_band` - `present_proof_v1_0` - `present_proof_v2_0` - `resolver` -
-`revocation` - `schema` - `server` - `trustping` - `wallet` ## Contributing If
-you would like to contribute to the framework, please read [CONTRIBUTING](/
-CONTRIBUTING.md) guidelines. These documents will provide more information to
-get you started! ## License Aries Cloud Controller Python is licensed under the
-[Apache License Version 2.0 (Apache-2.0)](/LICENSE).
+0.6.3 | 0.7.4 | | 0.7.0 | 0.7.5 | | 0.8.0 | 0.8.0 | | 0.8.1 | 0.8.1 | ##
+Features Aries Cloud Controller Python is a fully featured client for
+interacting with ACA-Py. - Fully Typed wrapper around Aries Cloud Agent Python
+- Supports latest ACA-Py version (0.8.1) - Client is auto generated based on
+OpenAPI definitions, allowing us to keep up to date with new releases. -
+Supports multi-tenant APIs and authentication - Async API ## Usage Aries Cloud
+Controller Python is published to PyPi and can be installed using pip: ```sh
+pip install aries-cloudcontroller ``` ### Creating a client ```python from
+aries_cloudcontroller import AcaPyClient client = AcaPyClient( base_url="http:/
+/localhost:8000", api_key="myApiKey" ) ``` **Admin insecure mode** If you are
+running ACA-Py with the admin insecure flag and don't have the API key, you
+must set the `admin_insecure` property: ```python client = AcaPyClient
+( base_url="http://localhost:8000", # Explicitly mark that no api key is used
+admin_insecure=True ) ``` **Multitenancy** To provision the agent in the
+context of specific tenant of the agent, the `tenant_jwt` property must be set:
+```python client = AcaPyClient( base_url="http://localhost:8000",
+tenant_jwt="eyXXX" ) ``` ### Interacting with the client Once you have the
+client set up, you're ready to interact with it. Because the API is fully
+typed, the best way to know what is available is by looking at the ACA-Py
+swagger UI, and the available properties on the client. For example to create
+and receive an invitation the following methods can be called: ```python
+invitation = await client.connection.create_invitation
+( body=CreateInvitationRequest(my_label="Cloud Controller") ) connection =
+await client.connection.receive_invitation(body=result.invitation) ``` ##
+Available APIs Currently the following top-level APIs are available in the
+client. Each api maps to the topics as used by the ACA-Py swagger UI. -
+`action_menu` - `basicmessage` - `connection` - `credential_definition` -
+`credentials` - `default` - `did_exchange` - `discover_features` -
+`discover_features_v2_0` - `endorse_transaction` - `introduction` -
+`issue_credential_v1_0` - `issue_credential_v2_0` - `jsonld` - `ledger` -
+`mediation` - `multitenancy` - `out_of_band` - `present_proof_v1_0` -
+`present_proof_v2_0` - `resolver` - `revocation` - `schema` - `server` -
+`trustping` - `wallet` ## Contributing If you would like to contribute to the
+framework, please read [CONTRIBUTING](/CONTRIBUTING.md) guidelines. These
+documents will provide more information to get you started! ## License Aries
+Cloud Controller Python is licensed under the [Apache License Version 2.0
+(Apache-2.0)](/LICENSE).
```

### Comparing `aries_cloudcontroller-0.8.0rc9/aries_cloudcontroller.egg-info/SOURCES.txt` & `aries_cloudcontroller-0.8.1rc4/aries_cloudcontroller.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -305,12 +305,19 @@
 aries_cloudcontroller/model/verify_request.py
 aries_cloudcontroller/model/verify_response.py
 aries_cloudcontroller/model/w3_c_credentials_list_request.py
 aries_cloudcontroller/model/wallet_list.py
 aries_cloudcontroller/model/wallet_record.py
 aries_cloudcontroller/model/write_ledger_request.py
 aries_cloudcontroller/util/__init__.py
+aries_cloudcontroller/util/create_client_session.py
 aries_cloudcontroller/util/pydantic_converter.py
 tests/__init__.py
+tests/compare_dicts.py
+tests/conftest.py
 tests/test_acapy_client.py
 tests/model/__init__.py
-tests/model/test_presentation.py
+tests/model/test_credential_offer.py
+tests/model/test_invitation.py
+tests/model/test_presentation.py
+tests/model/test_v20_cred_ex_record.py
+tests/model/test_v20_pres_ex_record.py
```

### Comparing `aries_cloudcontroller-0.8.0rc9/setup.py` & `aries_cloudcontroller-0.8.1rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.8.0-rc9",
+        version="0.8.1-rc4",
         description="A simple python package for controlling an aries agent through the admin-api interface",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/didx-xyz/aries-cloudcontroller-python/tree/main/aries_cloudcontroller",
         packages=find_packages(),
         include_package_data=True,
         package_data={
```

### Comparing `aries_cloudcontroller-0.8.0rc9/tests/model/test_presentation.py` & `aries_cloudcontroller-0.8.1rc4/tests/model/test_presentation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,18 @@
+import logging
+
 import pydantic
 import pytest
-import logging
 
-from aries_cloudcontroller.model.v10_presentation_exchange import (
-    V10PresentationExchange,
-)
+from aries_cloudcontroller.model import V10PresentationExchange
+from tests.compare_dicts import equal_dicts
 
 LOGGER = logging.getLogger(__name__)
 
-presentation_keys = [
-    "auto_present",
-    "connection_id",
-    "created_at",
-    "error_msg",
-    "initiator",
-    "presentation",
-    "presentation_exchange_id",
-    "presentation_proposal_dict",
-    "presentation_request",
-    "presentation_request_dict",
-    "role",
-    "state",
-    "thread_id",
-    "trace",
-    "updated_at",
-    "verified",
-]
-
-# From sample response in Swagger UI
-valid_presentation = {
+sample_presentation = {
     "auto_present": "false",
     "connection_id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
     "created_at": "2021-04-08 09:04:01Z",
     "error_msg": "Invalid structure",
     "initiator": "self",
     "presentation": {},
     "presentation_exchange_id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
@@ -45,18 +25,38 @@
     "state": "verified",
     "thread_id": "3fa85f64-5717-4562-b3fc-2c963f66afa6",
     "trace": "true",
     "updated_at": "2021-04-08 09:04:01Z",
     "verified": "true",
 }
 
-invalid_presentation = {"abc": "1234"}
+invalid_presentation = {
+    "auto_present": "",  # should be bool
+    "auto_verify": "",  # should be bool
+    "connection_id": [],  # should be str
+    "created_at": [],  # should be str
+    "error_msg": [],  # should be str
+    "initiator": "other",  # should be one of literal
+    "presentation": "invalid",  # should be dict
+    "presentation_exchange_id": [],  # should be str
+    "presentation_proposal_dict": "",  # should be dict
+    "presentation_request": "",  # should be dict
+    "presentation_request_dict": "",  # should be dict
+    "role": "other",  # should be one of literal
+    "state": [],  # should be str
+    "thread_id": [],  # should be str
+    "trace": "",  # should be list
+    "updated_at": [],  # should be str
+    "verified": "other",  # should be one of literal
+    "verified_msgs": "",  # should be list
+}
 
 
-def test_init_valid():
-    # Should not throw validation errors
-    V10PresentationExchange(**valid_presentation)
+def test_valid():
+    model = V10PresentationExchange(**sample_presentation)
+    assert equal_dicts(sample_presentation, model.dict(by_alias=True))
 
 
-def test_init_invalid():
-    with pytest.raises(pydantic.error_wrappers.ValidationError):
-        V10PresentationExchange(role="random")
+def test_invalid():
+    for key, value in invalid_presentation.items():
+        with pytest.raises(pydantic.error_wrappers.ValidationError):
+            V10PresentationExchange(**{key: value})
```

### Comparing `aries_cloudcontroller-0.8.0rc9/tests/test_acapy_client.py` & `aries_cloudcontroller-0.8.1rc4/tests/test_acapy_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 LOGGER = logging.getLogger(__name__)
 
 
 class TestAcaPyClient:
     admin_host = "http://localhost:1000"
     api_key = "api_key"
 
-    @pytest.mark.asyncio
+    @pytest.mark.anyio
     async def test_init_acapy_client(self):
         client = AcaPyClient(self.admin_host, api_key=self.api_key)
         assert type(client) is AcaPyClient
 
-    @pytest.mark.asyncio
+    @pytest.mark.anyio
     async def test_init_args_missing_api_key_no_insecure_mode(self):
         with pytest.raises(
             Exception,
             match=re.escape("api_key property is missing"),
         ):
             AcaPyClient(self.admin_host)
```

