# Comparing `tmp/calendly-py-0.0.1.tar.gz` & `tmp/calendly-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendly-py-0.0.1.tar", last modified: Tue Apr 11 11:57:57 2023, max compression
+gzip compressed data, was "calendly-py-0.0.2.tar", last modified: Tue Apr 11 12:19:03 2023, max compression
```

## Comparing `calendly-py-0.0.1.tar` & `calendly-py-0.0.2.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.827494 calendly-py-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 11:57:49.000000 calendly-py-0.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-11 11:57:57.827494 calendly-py-0.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2816 2023-04-11 11:57:49.000000 calendly-py-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:57:57.827494 calendly-py-0.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-04-11 11:57:49.000000 calendly-py-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.815494 calendly-py-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.819494 calendly-py-0.0.1/src/calendly_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-11 11:57:57.000000 calendly-py-0.0.1/src/calendly_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-11 11:57:57.000000 calendly-py-0.0.1/src/calendly_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:57:57.000000 calendly-py-0.0.1/src/calendly_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 11:57:57.000000 calendly-py-0.0.1/src/calendly_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 11:57:57.000000 calendly-py-0.0.1/src/calendly_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.819494 calendly-py-0.0.1/src/sdk/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/activity_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6682 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/availability.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5334 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/data_compliance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5668 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/event_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.819494 calendly-py-0.0.1/src/sdk/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.823494 calendly-py-0.0.1/src/sdk/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11380 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/delete_organizations_uuid_memberships.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/delete_users_user_uuid_webhooks_webhook_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/deleteinviteenoshow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2383 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_event_types_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2869 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_organizations_org_uuid_invitations_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4317 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_organizations_uuid_invitations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_organizations_uuid_memberships.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_routing_form_submissions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2556 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_routing_form_submissions_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2414 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_routing_forms_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3121 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_scheduled_events_event_uuid_invitees_invitee_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_scheduled_events_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/get_users_user_uuid_webhooks_webhook_uuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3092 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/geteventtypeavailabletimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2400 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getinviteenoshow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4887 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getinvitees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2374 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getuser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3664 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getuseravailabilityschedules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getuseravailabilityschedulesuuid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4114 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/getuserbusytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8072 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/list_activity_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/list_organization_memberships.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3431 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/list_routing_forms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5168 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/list_webhooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5510 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/listeventtypes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6504 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/listscheduledevents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2069 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/me.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3069 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_data_compliance_deletion_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2352 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_data_compliance_deletion_invitees.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5020 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_organizations_uuid_invitations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4567 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_scheduled_events_uuid_cancellation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4377 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_scheduling_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9556 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_shares.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5595 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/post_users_uuid_webhooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2522 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/postinviteenoshow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3768 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/operations/revoke_users_organization_invitation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.827494 calendly-py-0.0.1/src/sdk/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3878 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/actor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/availabilityrule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1526 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/availabilityschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/cancellation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1019 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/customlocation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2697 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/errorresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5219 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/event.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7217 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/eventtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/eventtypeavailabletime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2531 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/eventtypecustomquestion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1379 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/googleconference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/gotomeetingconference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/guest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      943 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inboundcall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inpersonmeeting.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/invitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1129 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inviteenoshow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      929 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inviteequestionandanswer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inviteespecifiedlocation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/inviteetracking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1071 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/legacycalendarevent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2951 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/microsoftteamsconference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2871 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/organizationinvitation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4237 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/organizationmembership.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/outboundcall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/pagination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/profile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1719 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/question.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2315 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/routingform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3195 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/routingformsubmission.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7909 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/share.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1649 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/submissioncustommessageresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1031 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/submissioneventtyperesult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/submissionexternalurlresult.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/submissionquestionandanswer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/submissiontracking.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2687 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/userbusytime.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/webexconference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3664 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/webhooksubscription.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4253 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/models/shared/zoomconference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11757 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/organizations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6334 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/routing_forms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14243 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/scheduled_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/scheduling_links.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5820 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2516 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/shares.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4783 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:57:57.827494 calendly-py-0.0.1/src/sdk/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7693 2023-04-11 11:57:49.000000 calendly-py-0.0.1/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.143760 calendly-py-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-11 12:18:43.000000 calendly-py-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-11 12:19:03.143760 calendly-py-0.0.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2812 2023-04-11 12:18:43.000000 calendly-py-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:19:03.143760 calendly-py-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1118 2023-04-11 12:18:43.000000 calendly-py-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.135760 calendly-py-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.135760 calendly-py-0.0.2/src/calendly/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2553 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/activity_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6687 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/availability.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5339 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/data_compliance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5673 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/event_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.135760 calendly-py-0.0.2/src/calendly/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.139760 calendly-py-0.0.2/src/calendly/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11340 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/delete_organizations_uuid_memberships.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2012 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/delete_users_user_uuid_webhooks_webhook_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1882 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/deleteinviteenoshow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2388 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_event_types_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2874 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_organizations_org_uuid_invitations_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4322 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_organizations_uuid_invitations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2802 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_organizations_uuid_memberships.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3540 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_routing_form_submissions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2561 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_routing_form_submissions_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2419 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_routing_forms_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3126 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_scheduled_events_event_uuid_invitees_invitee_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3542 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_scheduled_events_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2614 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/get_users_user_uuid_webhooks_webhook_uuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3097 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/geteventtypeavailabletimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2405 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getinviteenoshow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4892 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getinvitees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2379 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getuser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3669 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getuseravailabilityschedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3770 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getuseravailabilityschedulesuuid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4119 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/getuserbusytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8077 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/list_activity_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3905 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/list_organization_memberships.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3436 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/list_routing_forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5173 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/list_webhooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5515 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/listeventtypes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5970 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/listscheduledevents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2074 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/me.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3074 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_data_compliance_deletion_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2357 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_data_compliance_deletion_invitees.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5025 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_organizations_uuid_invitations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_scheduled_events_uuid_cancellation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4382 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_scheduling_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9561 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_shares.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5600 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/post_users_uuid_webhooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2527 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/postinviteenoshow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3773 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/operations/revoke_users_organization_invitation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.143760 calendly-py-0.0.2/src/calendly/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4525 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3883 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2605 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/availabilityrule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1531 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/availabilityschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/cancellation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/customlocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/errorresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5224 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/event.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7222 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/eventtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1564 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/eventtypeavailabletime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/eventtypecustomquestion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/googleconference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2256 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/gotomeetingconference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/guest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      948 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inboundcall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inpersonmeeting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9740 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/invitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inviteenoshow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inviteequestionandanswer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inviteespecifiedlocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/inviteetracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/legacycalendarevent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2956 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/microsoftteamsconference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2876 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/organizationinvitation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4242 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/organizationmembership.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/outboundcall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/pagination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1249 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1724 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/question.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2320 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/routingform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3200 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/routingformsubmission.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/scheduledeventsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7914 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/share.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/submissioncustommessageresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/submissioneventtyperesult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/submissionexternalurlresult.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/submissionquestionandanswer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1622 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/submissiontracking.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2692 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2845 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/userbusytime.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2941 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/webexconference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3669 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/webhooksubscription.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4258 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/models/shared/zoomconference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11762 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/organizations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6339 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/routing_forms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14206 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/scheduled_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2458 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/scheduling_links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5830 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/shares.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4788 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.143760 calendly-py-0.0.2/src/calendly/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7698 2023-04-11 12:18:43.000000 calendly-py-0.0.2/src/calendly/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:19:03.143760 calendly-py-0.0.2/src/calendly_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-11 12:19:02.000000 calendly-py-0.0.2/src/calendly_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-11 12:19:03.000000 calendly-py-0.0.2/src/calendly_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:19:02.000000 calendly-py-0.0.2/src/calendly_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 12:19:02.000000 calendly-py-0.0.2/src/calendly_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 12:19:02.000000 calendly-py-0.0.2/src/calendly_py.egg-info/top_level.txt
```

### Comparing `calendly-py-0.0.1/LICENSE.md` & `calendly-py-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendly-py-0.0.1/PKG-INFO` & `calendly-py-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendly-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for the calendly API Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,18 +19,18 @@
 pip install calendly-py
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import sdk
-from sdk.models import operations, shared
+import calendly
+from calendly.models import operations, shared
 
-s = sdk.SDK(
+s = calendly.Calendly(
     security=shared.Security(
         oauth2="Bearer YOUR_ACCESS_TOKEN_HERE",
     ),
 )
 
 
 req = operations.ListScheduledEventsRequest(
@@ -43,15 +43,15 @@
     sort="unde",
     status="canceled",
     user="https://api.calendly.com/users/EBHAAFHDCAEQTSEZ",
 )
     
 res = s.scheduled_events.list(req)
 
-if res.list_scheduled_events_200_application_json_object is not None:
+if res.scheduled_events_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
```

### Comparing `calendly-py-0.0.1/README.md` & `calendly-py-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 pip install calendly-py
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import sdk
-from sdk.models import operations, shared
+import calendly
+from calendly.models import operations, shared
 
-s = sdk.SDK(
+s = calendly.Calendly(
     security=shared.Security(
         oauth2="Bearer YOUR_ACCESS_TOKEN_HERE",
     ),
 )
 
 
 req = operations.ListScheduledEventsRequest(
@@ -31,15 +31,15 @@
     sort="unde",
     status="canceled",
     user="https://api.calendly.com/users/EBHAAFHDCAEQTSEZ",
 )
     
 res = s.scheduled_events.list(req)
 
-if res.list_scheduled_events_200_application_json_object is not None:
+if res.scheduled_events_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
```

### Comparing `calendly-py-0.0.1/setup.py` & `calendly-py-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="calendly-py",
-    version="0.0.1",
+    version="0.0.2",
     author="Speakeasy",
     description="Python SDK for the calendly API Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `calendly-py-0.0.1/src/calendly_py.egg-info/PKG-INFO` & `calendly-py-0.0.2/src/calendly_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calendly-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for the calendly API Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -19,18 +19,18 @@
 pip install calendly-py
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
-import sdk
-from sdk.models import operations, shared
+import calendly
+from calendly.models import operations, shared
 
-s = sdk.SDK(
+s = calendly.Calendly(
     security=shared.Security(
         oauth2="Bearer YOUR_ACCESS_TOKEN_HERE",
     ),
 )
 
 
 req = operations.ListScheduledEventsRequest(
@@ -43,15 +43,15 @@
     sort="unde",
     status="canceled",
     user="https://api.calendly.com/users/EBHAAFHDCAEQTSEZ",
 )
     
 res = s.scheduled_events.list(req)
 
-if res.list_scheduled_events_200_application_json_object is not None:
+if res.scheduled_events_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
```

### Comparing `calendly-py-0.0.1/src/sdk/activity_log.py` & `calendly-py-0.0.2/src/calendly/activity_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class ActivityLog:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/availability.py` & `calendly-py-0.0.2/src/calendly/availability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations, shared
+from calendly.models import operations, shared
 from typing import Optional
 
 class Availability:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/data_compliance.py` & `calendly-py-0.0.2/src/calendly/data_compliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations, shared
+from calendly.models import operations, shared
 from typing import Any, Optional
 
 class DataCompliance:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/event_types.py` & `calendly-py-0.0.2/src/calendly/event_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class EventTypes:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/__init__.py` & `calendly-py-0.0.2/src/calendly/models/operations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 from .post_scheduled_events_uuid_cancellation import *
 from .post_scheduling_links import *
 from .post_shares import *
 from .post_users_uuid_webhooks import *
 from .postinviteenoshow import *
 from .revoke_users_organization_invitation import *
 
-__all__ = ["DeleteInviteeNoShowErrorResponse","DeleteInviteeNoShowErrorResponseDetails","DeleteInviteeNoShowRequest","DeleteInviteeNoShowResponse","DeleteOrganizationsUUIDMembershipsErrorResponse","DeleteOrganizationsUUIDMembershipsErrorResponseDetails","DeleteOrganizationsUUIDMembershipsRequest","DeleteOrganizationsUUIDMembershipsResponse","DeleteUsersUserUUIDWebhooksWebhookUUIDErrorResponse","DeleteUsersUserUUIDWebhooksWebhookUUIDErrorResponseDetails","DeleteUsersUserUUIDWebhooksWebhookUUIDRequest","DeleteUsersUserUUIDWebhooksWebhookUUIDResponse","GetEventTypeAvailableTimes200ApplicationJSON","GetEventTypeAvailableTimesErrorResponse","GetEventTypeAvailableTimesErrorResponseDetails","GetEventTypeAvailableTimesRequest","GetEventTypeAvailableTimesResponse","GetEventTypesUUID200ApplicationJSON","GetEventTypesUUIDErrorResponse","GetEventTypesUUIDErrorResponseDetails","GetEventTypesUUIDRequest","GetEventTypesUUIDResponse","GetInviteeNoShow200ApplicationJSON","GetInviteeNoShowErrorResponse","GetInviteeNoShowErrorResponseDetails","GetInviteeNoShowRequest","GetInviteeNoShowResponse","GetInvitees200ApplicationJSON","GetInvitees403ApplicationJSON","GetInvitees403ApplicationJSONMessageEnum","GetInvitees403ApplicationJSONTitleEnum","GetInviteesErrorResponse","GetInviteesErrorResponseDetails","GetInviteesRequest","GetInviteesResponse","GetInviteesStatusEnum","GetOrganizationsOrgUUIDInvitationsUUID200ApplicationJSON","GetOrganizationsOrgUUIDInvitationsUUIDErrorResponse","GetOrganizationsOrgUUIDInvitationsUUIDErrorResponseDetails","GetOrganizationsOrgUUIDInvitationsUUIDRequest","GetOrganizationsOrgUUIDInvitationsUUIDResponse","GetOrganizationsUUIDInvitations200ApplicationJSON","GetOrganizationsUUIDInvitationsErrorResponse","GetOrganizationsUUIDInvitationsErrorResponseDetails","GetOrganizationsUUIDInvitationsRequest","GetOrganizationsUUIDInvitationsResponse","GetOrganizationsUUIDInvitationsStatusEnum","GetOrganizationsUUIDMemberships200ApplicationJSON","GetOrganizationsUUIDMembershipsErrorResponse","GetOrganizationsUUIDMembershipsErrorResponseDetails","GetOrganizationsUUIDMembershipsRequest","GetOrganizationsUUIDMembershipsResponse","GetRoutingFormSubmissions200ApplicationJSON","GetRoutingFormSubmissionsErrorResponse","GetRoutingFormSubmissionsErrorResponseDetails","GetRoutingFormSubmissionsRequest","GetRoutingFormSubmissionsResponse","GetRoutingFormSubmissionsUUID200ApplicationJSON","GetRoutingFormSubmissionsUUIDErrorResponse","GetRoutingFormSubmissionsUUIDErrorResponseDetails","GetRoutingFormSubmissionsUUIDRequest","GetRoutingFormSubmissionsUUIDResponse","GetRoutingFormsUUID200ApplicationJSON","GetRoutingFormsUUIDErrorResponse","GetRoutingFormsUUIDErrorResponseDetails","GetRoutingFormsUUIDRequest","GetRoutingFormsUUIDResponse","GetScheduledEventsEventUUIDInviteesInviteeUUID200ApplicationJSON","GetScheduledEventsEventUUIDInviteesInviteeUUIDErrorResponse","GetScheduledEventsEventUUIDInviteesInviteeUUIDErrorResponseDetails","GetScheduledEventsEventUUIDInviteesInviteeUUIDRequest","GetScheduledEventsEventUUIDInviteesInviteeUUIDResponse","GetScheduledEventsUUID200ApplicationJSON","GetScheduledEventsUUID403ApplicationJSON","GetScheduledEventsUUID403ApplicationJSONMessageEnum","GetScheduledEventsUUID403ApplicationJSONTitleEnum","GetScheduledEventsUUIDErrorResponse","GetScheduledEventsUUIDErrorResponseDetails","GetScheduledEventsUUIDRequest","GetScheduledEventsUUIDResponse","GetUser200ApplicationJSON","GetUserAvailabilitySchedules200ApplicationJSON","GetUserAvailabilitySchedules403ApplicationJSON","GetUserAvailabilitySchedules403ApplicationJSONMessageEnum","GetUserAvailabilitySchedules403ApplicationJSONTitleEnum","GetUserAvailabilitySchedulesErrorResponse","GetUserAvailabilitySchedulesErrorResponseDetails","GetUserAvailabilitySchedulesRequest","GetUserAvailabilitySchedulesResponse","GetUserAvailabilitySchedulesUUID200ApplicationJSON","GetUserAvailabilitySchedulesUUID403ApplicationJSON","GetUserAvailabilitySchedulesUUID403ApplicationJSONMessageEnum","GetUserAvailabilitySchedulesUUID403ApplicationJSONTitleEnum","GetUserAvailabilitySchedulesUUIDErrorResponse","GetUserAvailabilitySchedulesUUIDErrorResponseDetails","GetUserAvailabilitySchedulesUUIDRequest","GetUserAvailabilitySchedulesUUIDResponse","GetUserBusyTimes200ApplicationJSON","GetUserBusyTimes403ApplicationJSON","GetUserBusyTimes403ApplicationJSONMessageEnum","GetUserBusyTimes403ApplicationJSONTitleEnum","GetUserBusyTimesErrorResponse","GetUserBusyTimesErrorResponseDetails","GetUserBusyTimesRequest","GetUserBusyTimesResponse","GetUserErrorResponse","GetUserErrorResponseDetails","GetUserRequest","GetUserResponse","GetUsersUserUUIDWebhooksWebhookUUID200ApplicationJSON","GetUsersUserUUIDWebhooksWebhookUUIDErrorResponse","GetUsersUserUUIDWebhooksWebhookUUIDErrorResponseDetails","GetUsersUserUUIDWebhooksWebhookUUIDRequest","GetUsersUserUUIDWebhooksWebhookUUIDResponse","ListActivityLog200ApplicationJSON","ListActivityLog403ApplicationJSON","ListActivityLog403ApplicationJSONMessageEnum","ListActivityLog403ApplicationJSONTitleEnum","ListActivityLogErrorResponse","ListActivityLogErrorResponseDetails","ListActivityLogRequest","ListActivityLogResponse","ListActivityLogSortEnum","ListEventTypes200ApplicationJSON","ListEventTypes403ApplicationJSON","ListEventTypes403ApplicationJSONMessageEnum","ListEventTypes403ApplicationJSONTitleEnum","ListEventTypesErrorResponse","ListEventTypesErrorResponseDetails","ListEventTypesRequest","ListEventTypesResponse","ListOrganizationMemberships200ApplicationJSON","ListOrganizationMembershipsErrorResponse","ListOrganizationMembershipsErrorResponseDetails","ListOrganizationMembershipsRequest","ListOrganizationMembershipsResponse","ListRoutingForms200ApplicationJSON","ListRoutingFormsErrorResponse","ListRoutingFormsErrorResponseDetails","ListRoutingFormsRequest","ListRoutingFormsResponse","ListScheduledEvents200ApplicationJSON","ListScheduledEvents403ApplicationJSON","ListScheduledEvents403ApplicationJSONMessageEnum","ListScheduledEvents403ApplicationJSONTitleEnum","ListScheduledEventsErrorResponse","ListScheduledEventsErrorResponseDetails","ListScheduledEventsRequest","ListScheduledEventsResponse","ListScheduledEventsStatusEnum","ListWebhooks200ApplicationJSON","ListWebhooks403ApplicationJSON","ListWebhooks403ApplicationJSONMessageEnum","ListWebhooks403ApplicationJSONTitleEnum","ListWebhooksErrorResponse","ListWebhooksErrorResponseDetails","ListWebhooksRequest","ListWebhooksResponse","ListWebhooksScopeEnum","Me200ApplicationJSON","MeErrorResponse","MeErrorResponseDetails","MeResponse","PostDataComplianceDeletionEventsErrorResponse","PostDataComplianceDeletionEventsErrorResponseDetails","PostDataComplianceDeletionEventsRequestBody","PostDataComplianceDeletionEventsResponse","PostDataComplianceDeletionInviteesErrorResponse","PostDataComplianceDeletionInviteesErrorResponseDetails","PostDataComplianceDeletionInviteesRequestBody","PostDataComplianceDeletionInviteesResponse","PostInviteeNoShow201ApplicationJSON","PostInviteeNoShowErrorResponse","PostInviteeNoShowErrorResponseDetails","PostInviteeNoShowRequestBody","PostInviteeNoShowResponse","PostOrganizationsUUIDInvitations201ApplicationJSON","PostOrganizationsUUIDInvitations403ApplicationJSON","PostOrganizationsUUIDInvitations403ApplicationJSONMessageEnum","PostOrganizationsUUIDInvitations403ApplicationJSONTitleEnum","PostOrganizationsUUIDInvitationsErrorResponse","PostOrganizationsUUIDInvitationsErrorResponseDetails","PostOrganizationsUUIDInvitationsRequest","PostOrganizationsUUIDInvitationsRequestBody","PostOrganizationsUUIDInvitationsResponse","PostScheduledEventsUUIDCancellation201ApplicationJSON","PostScheduledEventsUUIDCancellation403ApplicationJSON","PostScheduledEventsUUIDCancellation403ApplicationJSONMessageEnum","PostScheduledEventsUUIDCancellation403ApplicationJSONTitleEnum","PostScheduledEventsUUIDCancellationApplicationJSON","PostScheduledEventsUUIDCancellationErrorResponse","PostScheduledEventsUUIDCancellationErrorResponseDetails","PostScheduledEventsUUIDCancellationRequest","PostScheduledEventsUUIDCancellationResponse","PostSchedulingLinks201ApplicationJSON","PostSchedulingLinks201ApplicationJSONResource","PostSchedulingLinks201ApplicationJSONResourceOwnerTypeEnum","PostSchedulingLinksErrorResponse","PostSchedulingLinksErrorResponseDetails","PostSchedulingLinksRequestBody","PostSchedulingLinksRequestBodyMaxEventCountEnum","PostSchedulingLinksRequestBodyOwnerTypeEnum","PostSchedulingLinksResponse","PostShares201ApplicationJSON","PostSharesErrorResponse","PostSharesErrorResponseDetails","PostSharesRequestBody","PostSharesRequestBodyAvailabilityRule","PostSharesRequestBodyAvailabilityRuleRules","PostSharesRequestBodyAvailabilityRuleRulesIntervals","PostSharesRequestBodyAvailabilityRuleRulesTypeEnum","PostSharesRequestBodyAvailabilityRuleRulesWdayEnum","PostSharesRequestBodyLocationConfigurations","PostSharesRequestBodyLocationConfigurationsKindEnum","PostSharesRequestBodyPeriodTypeEnum","PostSharesResponse","PostUsersUUIDWebhooks201ApplicationJSON","PostUsersUUIDWebhooks403ApplicationJSON","PostUsersUUIDWebhooks403ApplicationJSONMessageEnum","PostUsersUUIDWebhooks403ApplicationJSONTitleEnum","PostUsersUUIDWebhooksErrorResponse","PostUsersUUIDWebhooksErrorResponseDetails","PostUsersUUIDWebhooksRequestBody","PostUsersUUIDWebhooksRequestBodyEventsEnum","PostUsersUUIDWebhooksRequestBodyScopeEnum","PostUsersUUIDWebhooksResponse","RevokeUsersOrganizationInvitation403ApplicationJSON","RevokeUsersOrganizationInvitation403ApplicationJSONMessageEnum","RevokeUsersOrganizationInvitation403ApplicationJSONTitleEnum","RevokeUsersOrganizationInvitationErrorResponse","RevokeUsersOrganizationInvitationErrorResponseDetails","RevokeUsersOrganizationInvitationRequest","RevokeUsersOrganizationInvitationResponse"]
+__all__ = ["DeleteInviteeNoShowErrorResponse","DeleteInviteeNoShowErrorResponseDetails","DeleteInviteeNoShowRequest","DeleteInviteeNoShowResponse","DeleteOrganizationsUUIDMembershipsErrorResponse","DeleteOrganizationsUUIDMembershipsErrorResponseDetails","DeleteOrganizationsUUIDMembershipsRequest","DeleteOrganizationsUUIDMembershipsResponse","DeleteUsersUserUUIDWebhooksWebhookUUIDErrorResponse","DeleteUsersUserUUIDWebhooksWebhookUUIDErrorResponseDetails","DeleteUsersUserUUIDWebhooksWebhookUUIDRequest","DeleteUsersUserUUIDWebhooksWebhookUUIDResponse","GetEventTypeAvailableTimes200ApplicationJSON","GetEventTypeAvailableTimesErrorResponse","GetEventTypeAvailableTimesErrorResponseDetails","GetEventTypeAvailableTimesRequest","GetEventTypeAvailableTimesResponse","GetEventTypesUUID200ApplicationJSON","GetEventTypesUUIDErrorResponse","GetEventTypesUUIDErrorResponseDetails","GetEventTypesUUIDRequest","GetEventTypesUUIDResponse","GetInviteeNoShow200ApplicationJSON","GetInviteeNoShowErrorResponse","GetInviteeNoShowErrorResponseDetails","GetInviteeNoShowRequest","GetInviteeNoShowResponse","GetInvitees200ApplicationJSON","GetInvitees403ApplicationJSON","GetInvitees403ApplicationJSONMessageEnum","GetInvitees403ApplicationJSONTitleEnum","GetInviteesErrorResponse","GetInviteesErrorResponseDetails","GetInviteesRequest","GetInviteesResponse","GetInviteesStatusEnum","GetOrganizationsOrgUUIDInvitationsUUID200ApplicationJSON","GetOrganizationsOrgUUIDInvitationsUUIDErrorResponse","GetOrganizationsOrgUUIDInvitationsUUIDErrorResponseDetails","GetOrganizationsOrgUUIDInvitationsUUIDRequest","GetOrganizationsOrgUUIDInvitationsUUIDResponse","GetOrganizationsUUIDInvitations200ApplicationJSON","GetOrganizationsUUIDInvitationsErrorResponse","GetOrganizationsUUIDInvitationsErrorResponseDetails","GetOrganizationsUUIDInvitationsRequest","GetOrganizationsUUIDInvitationsResponse","GetOrganizationsUUIDInvitationsStatusEnum","GetOrganizationsUUIDMemberships200ApplicationJSON","GetOrganizationsUUIDMembershipsErrorResponse","GetOrganizationsUUIDMembershipsErrorResponseDetails","GetOrganizationsUUIDMembershipsRequest","GetOrganizationsUUIDMembershipsResponse","GetRoutingFormSubmissions200ApplicationJSON","GetRoutingFormSubmissionsErrorResponse","GetRoutingFormSubmissionsErrorResponseDetails","GetRoutingFormSubmissionsRequest","GetRoutingFormSubmissionsResponse","GetRoutingFormSubmissionsUUID200ApplicationJSON","GetRoutingFormSubmissionsUUIDErrorResponse","GetRoutingFormSubmissionsUUIDErrorResponseDetails","GetRoutingFormSubmissionsUUIDRequest","GetRoutingFormSubmissionsUUIDResponse","GetRoutingFormsUUID200ApplicationJSON","GetRoutingFormsUUIDErrorResponse","GetRoutingFormsUUIDErrorResponseDetails","GetRoutingFormsUUIDRequest","GetRoutingFormsUUIDResponse","GetScheduledEventsEventUUIDInviteesInviteeUUID200ApplicationJSON","GetScheduledEventsEventUUIDInviteesInviteeUUIDErrorResponse","GetScheduledEventsEventUUIDInviteesInviteeUUIDErrorResponseDetails","GetScheduledEventsEventUUIDInviteesInviteeUUIDRequest","GetScheduledEventsEventUUIDInviteesInviteeUUIDResponse","GetScheduledEventsUUID200ApplicationJSON","GetScheduledEventsUUID403ApplicationJSON","GetScheduledEventsUUID403ApplicationJSONMessageEnum","GetScheduledEventsUUID403ApplicationJSONTitleEnum","GetScheduledEventsUUIDErrorResponse","GetScheduledEventsUUIDErrorResponseDetails","GetScheduledEventsUUIDRequest","GetScheduledEventsUUIDResponse","GetUser200ApplicationJSON","GetUserAvailabilitySchedules200ApplicationJSON","GetUserAvailabilitySchedules403ApplicationJSON","GetUserAvailabilitySchedules403ApplicationJSONMessageEnum","GetUserAvailabilitySchedules403ApplicationJSONTitleEnum","GetUserAvailabilitySchedulesErrorResponse","GetUserAvailabilitySchedulesErrorResponseDetails","GetUserAvailabilitySchedulesRequest","GetUserAvailabilitySchedulesResponse","GetUserAvailabilitySchedulesUUID200ApplicationJSON","GetUserAvailabilitySchedulesUUID403ApplicationJSON","GetUserAvailabilitySchedulesUUID403ApplicationJSONMessageEnum","GetUserAvailabilitySchedulesUUID403ApplicationJSONTitleEnum","GetUserAvailabilitySchedulesUUIDErrorResponse","GetUserAvailabilitySchedulesUUIDErrorResponseDetails","GetUserAvailabilitySchedulesUUIDRequest","GetUserAvailabilitySchedulesUUIDResponse","GetUserBusyTimes200ApplicationJSON","GetUserBusyTimes403ApplicationJSON","GetUserBusyTimes403ApplicationJSONMessageEnum","GetUserBusyTimes403ApplicationJSONTitleEnum","GetUserBusyTimesErrorResponse","GetUserBusyTimesErrorResponseDetails","GetUserBusyTimesRequest","GetUserBusyTimesResponse","GetUserErrorResponse","GetUserErrorResponseDetails","GetUserRequest","GetUserResponse","GetUsersUserUUIDWebhooksWebhookUUID200ApplicationJSON","GetUsersUserUUIDWebhooksWebhookUUIDErrorResponse","GetUsersUserUUIDWebhooksWebhookUUIDErrorResponseDetails","GetUsersUserUUIDWebhooksWebhookUUIDRequest","GetUsersUserUUIDWebhooksWebhookUUIDResponse","ListActivityLog200ApplicationJSON","ListActivityLog403ApplicationJSON","ListActivityLog403ApplicationJSONMessageEnum","ListActivityLog403ApplicationJSONTitleEnum","ListActivityLogErrorResponse","ListActivityLogErrorResponseDetails","ListActivityLogRequest","ListActivityLogResponse","ListActivityLogSortEnum","ListEventTypes200ApplicationJSON","ListEventTypes403ApplicationJSON","ListEventTypes403ApplicationJSONMessageEnum","ListEventTypes403ApplicationJSONTitleEnum","ListEventTypesErrorResponse","ListEventTypesErrorResponseDetails","ListEventTypesRequest","ListEventTypesResponse","ListOrganizationMemberships200ApplicationJSON","ListOrganizationMembershipsErrorResponse","ListOrganizationMembershipsErrorResponseDetails","ListOrganizationMembershipsRequest","ListOrganizationMembershipsResponse","ListRoutingForms200ApplicationJSON","ListRoutingFormsErrorResponse","ListRoutingFormsErrorResponseDetails","ListRoutingFormsRequest","ListRoutingFormsResponse","ListScheduledEvents403ApplicationJSON","ListScheduledEvents403ApplicationJSONMessageEnum","ListScheduledEvents403ApplicationJSONTitleEnum","ListScheduledEventsErrorResponse","ListScheduledEventsErrorResponseDetails","ListScheduledEventsRequest","ListScheduledEventsResponse","ListScheduledEventsStatusEnum","ListWebhooks200ApplicationJSON","ListWebhooks403ApplicationJSON","ListWebhooks403ApplicationJSONMessageEnum","ListWebhooks403ApplicationJSONTitleEnum","ListWebhooksErrorResponse","ListWebhooksErrorResponseDetails","ListWebhooksRequest","ListWebhooksResponse","ListWebhooksScopeEnum","Me200ApplicationJSON","MeErrorResponse","MeErrorResponseDetails","MeResponse","PostDataComplianceDeletionEventsErrorResponse","PostDataComplianceDeletionEventsErrorResponseDetails","PostDataComplianceDeletionEventsRequestBody","PostDataComplianceDeletionEventsResponse","PostDataComplianceDeletionInviteesErrorResponse","PostDataComplianceDeletionInviteesErrorResponseDetails","PostDataComplianceDeletionInviteesRequestBody","PostDataComplianceDeletionInviteesResponse","PostInviteeNoShow201ApplicationJSON","PostInviteeNoShowErrorResponse","PostInviteeNoShowErrorResponseDetails","PostInviteeNoShowRequestBody","PostInviteeNoShowResponse","PostOrganizationsUUIDInvitations201ApplicationJSON","PostOrganizationsUUIDInvitations403ApplicationJSON","PostOrganizationsUUIDInvitations403ApplicationJSONMessageEnum","PostOrganizationsUUIDInvitations403ApplicationJSONTitleEnum","PostOrganizationsUUIDInvitationsErrorResponse","PostOrganizationsUUIDInvitationsErrorResponseDetails","PostOrganizationsUUIDInvitationsRequest","PostOrganizationsUUIDInvitationsRequestBody","PostOrganizationsUUIDInvitationsResponse","PostScheduledEventsUUIDCancellation201ApplicationJSON","PostScheduledEventsUUIDCancellation403ApplicationJSON","PostScheduledEventsUUIDCancellation403ApplicationJSONMessageEnum","PostScheduledEventsUUIDCancellation403ApplicationJSONTitleEnum","PostScheduledEventsUUIDCancellationApplicationJSON","PostScheduledEventsUUIDCancellationErrorResponse","PostScheduledEventsUUIDCancellationErrorResponseDetails","PostScheduledEventsUUIDCancellationRequest","PostScheduledEventsUUIDCancellationResponse","PostSchedulingLinks201ApplicationJSON","PostSchedulingLinks201ApplicationJSONResource","PostSchedulingLinks201ApplicationJSONResourceOwnerTypeEnum","PostSchedulingLinksErrorResponse","PostSchedulingLinksErrorResponseDetails","PostSchedulingLinksRequestBody","PostSchedulingLinksRequestBodyMaxEventCountEnum","PostSchedulingLinksRequestBodyOwnerTypeEnum","PostSchedulingLinksResponse","PostShares201ApplicationJSON","PostSharesErrorResponse","PostSharesErrorResponseDetails","PostSharesRequestBody","PostSharesRequestBodyAvailabilityRule","PostSharesRequestBodyAvailabilityRuleRules","PostSharesRequestBodyAvailabilityRuleRulesIntervals","PostSharesRequestBodyAvailabilityRuleRulesTypeEnum","PostSharesRequestBodyAvailabilityRuleRulesWdayEnum","PostSharesRequestBodyLocationConfigurations","PostSharesRequestBodyLocationConfigurationsKindEnum","PostSharesRequestBodyPeriodTypeEnum","PostSharesResponse","PostUsersUUIDWebhooks201ApplicationJSON","PostUsersUUIDWebhooks403ApplicationJSON","PostUsersUUIDWebhooks403ApplicationJSONMessageEnum","PostUsersUUIDWebhooks403ApplicationJSONTitleEnum","PostUsersUUIDWebhooksErrorResponse","PostUsersUUIDWebhooksErrorResponseDetails","PostUsersUUIDWebhooksRequestBody","PostUsersUUIDWebhooksRequestBodyEventsEnum","PostUsersUUIDWebhooksRequestBodyScopeEnum","PostUsersUUIDWebhooksResponse","RevokeUsersOrganizationInvitation403ApplicationJSON","RevokeUsersOrganizationInvitation403ApplicationJSONMessageEnum","RevokeUsersOrganizationInvitation403ApplicationJSONTitleEnum","RevokeUsersOrganizationInvitationErrorResponse","RevokeUsersOrganizationInvitationErrorResponseDetails","RevokeUsersOrganizationInvitationRequest","RevokeUsersOrganizationInvitationResponse"]
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/delete_organizations_uuid_memberships.py` & `calendly-py-0.0.2/src/calendly/models/operations/delete_organizations_uuid_memberships.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteOrganizationsUUIDMembershipsRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/delete_users_user_uuid_webhooks_webhook_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/delete_users_user_uuid_webhooks_webhook_uuid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteUsersUserUUIDWebhooksWebhookUUIDRequest:
     
     webhook_uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'webhook_uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/deleteinviteenoshow.py` & `calendly-py-0.0.2/src/calendly/models/operations/deleteinviteenoshow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteInviteeNoShowRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_event_types_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_event_types_uuid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import eventtype as shared_eventtype
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetEventTypesUUIDRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_organizations_org_uuid_invitations_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_organizations_org_uuid_invitations_uuid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import organizationinvitation as shared_organizationinvitation
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetOrganizationsOrgUUIDInvitationsUUIDRequest:
     
     org_uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'org_uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_organizations_uuid_invitations.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_organizations_uuid_invitations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import organizationinvitation as shared_organizationinvitation
 from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class GetOrganizationsUUIDInvitationsStatusEnum(str, Enum):
     r"""Indicates if the results should be filtered by status  (\\"pending\\", \\"accepted\\", or \\"declined\\")"""
     PENDING = 'pending'
     ACCEPTED = 'accepted'
     DECLINED = 'declined'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_organizations_uuid_memberships.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_organizations_uuid_memberships.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import organizationmembership as shared_organizationmembership
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetOrganizationsUUIDMembershipsRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_routing_form_submissions.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_routing_form_submissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import pagination as shared_pagination
 from ..shared import routingformsubmission as shared_routingformsubmission
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetRoutingFormSubmissionsRequest:
     
     form: str = dataclasses.field(metadata={'query_param': { 'field_name': 'form', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_routing_form_submissions_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_routing_form_submissions_uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import routingformsubmission as shared_routingformsubmission
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetRoutingFormSubmissionsUUIDRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_routing_forms_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_routing_forms_uuid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import routingform as shared_routingform
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetRoutingFormsUUIDRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_scheduled_events_event_uuid_invitees_invitee_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_scheduled_events_event_uuid_invitees_invitee_uuid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import invitee as shared_invitee
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetScheduledEventsEventUUIDInviteesInviteeUUIDRequest:
     
     event_uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'event_uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_scheduled_events_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_scheduled_events_uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import event as shared_event
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetScheduledEventsUUIDRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/get_users_user_uuid_webhooks_webhook_uuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/get_users_user_uuid_webhooks_webhook_uuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import webhooksubscription as shared_webhooksubscription
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetUsersUserUUIDWebhooksWebhookUUIDRequest:
     
     webhook_uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'webhook_uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/geteventtypeavailabletimes.py` & `calendly-py-0.0.2/src/calendly/models/operations/geteventtypeavailabletimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import eventtypeavailabletime as shared_eventtypeavailabletime
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetEventTypeAvailableTimesRequest:
     
     end_time: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'end_time', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getinviteenoshow.py` & `calendly-py-0.0.2/src/calendly/models/operations/getinviteenoshow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import inviteenoshow as shared_inviteenoshow
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetInviteeNoShowRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getinvitees.py` & `calendly-py-0.0.2/src/calendly/models/operations/getinvitees.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import invitee as shared_invitee
 from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class GetInviteesStatusEnum(str, Enum):
     r"""Indicates if the invitee \\"canceled\\" or still \\"active\\" """
     ACTIVE = 'active'
     CANCELED = 'canceled'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getuser.py` & `calendly-py-0.0.2/src/calendly/models/operations/getuser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import user as shared_user
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetUserRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getuseravailabilityschedules.py` & `calendly-py-0.0.2/src/calendly/models/operations/getuseravailabilityschedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import availabilityschedule as shared_availabilityschedule
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetUserAvailabilitySchedulesRequest:
     
     user: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'user', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getuseravailabilityschedulesuuid.py` & `calendly-py-0.0.2/src/calendly/models/operations/getuseravailabilityschedulesuuid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import availabilityschedule as shared_availabilityschedule
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetUserAvailabilitySchedulesUUIDRequest:
     
     uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/getuserbusytimes.py` & `calendly-py-0.0.2/src/calendly/models/operations/getuserbusytimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import userbusytime as shared_userbusytime
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetUserBusyTimesRequest:
     
     end_time: str = dataclasses.field(metadata={'query_param': { 'field_name': 'end_time', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/list_activity_log.py` & `calendly-py-0.0.2/src/calendly/models/operations/list_activity_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 import requests as requests_http
 from ..shared import entry as shared_entry
 from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 class ListActivityLogSortEnum(str, Enum):
     ACTION_ASC = 'action:asc'
     ACTION_DESC = 'action:desc'
     ACTOR_DISPLAY_NAME_ASC = 'actor.display_name:asc'
     ACTOR_DISPLAY_NAME_DESC = 'actor.display_name:desc'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/list_organization_memberships.py` & `calendly-py-0.0.2/src/calendly/models/operations/list_organization_memberships.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import organizationmembership as shared_organizationmembership
 from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListOrganizationMembershipsRequest:
     
     count: Optional[float] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'count', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/list_routing_forms.py` & `calendly-py-0.0.2/src/calendly/models/operations/list_routing_forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import pagination as shared_pagination
 from ..shared import routingform as shared_routingform
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListRoutingFormsRequest:
     
     organization: str = dataclasses.field(metadata={'query_param': { 'field_name': 'organization', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/list_webhooks.py` & `calendly-py-0.0.2/src/calendly/models/operations/list_webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import pagination as shared_pagination
 from ..shared import webhooksubscription as shared_webhooksubscription
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class ListWebhooksScopeEnum(str, Enum):
     r"""Filter the list by organization or user"""
     ORGANIZATION = 'organization'
     USER = 'user'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/listeventtypes.py` & `calendly-py-0.0.2/src/calendly/models/operations/listeventtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import eventtype as shared_eventtype
 from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListEventTypesRequest:
     
     active: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'active', 'style': 'form', 'explode': True }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/listscheduledevents.py` & `calendly-py-0.0.2/src/calendly/models/operations/listscheduledevents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import event as shared_event
-from ..shared import pagination as shared_pagination
+from ..shared import scheduledeventsresponse as shared_scheduledeventsresponse
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class ListScheduledEventsStatusEnum(str, Enum):
     r"""Whether the scheduled event is `active` or `canceled`"""
     ACTIVE = 'active'
     CANCELED = 'canceled'
 
@@ -74,30 +73,20 @@
     r"""Error Object"""
     
     message: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message') }})  
     title: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('title') }})  
     details: Optional[list[ListScheduledEventsErrorResponseDetails]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})  
     
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListScheduledEvents200ApplicationJSON:
-    r"""Service response"""
-    
-    collection: list[shared_event.Event] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('collection') }})
-    r"""The set of scheduled events matching the criteria"""  
-    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})  
-    
-
 @dataclasses.dataclass
 class ListScheduledEventsResponse:
     
     content_type: str = dataclasses.field()  
     status_code: int = dataclasses.field()  
     error_response: Optional[ListScheduledEventsErrorResponse] = dataclasses.field(default=None)
     r"""Request is not valid"""  
-    list_scheduled_events_200_application_json_object: Optional[ListScheduledEvents200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""  
     list_scheduled_events_403_application_json_object: Optional[ListScheduledEvents403ApplicationJSON] = dataclasses.field(default=None)
     r"""Permission Denied"""  
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    scheduled_events_response: Optional[shared_scheduledeventsresponse.ScheduledEventsResponse] = dataclasses.field(default=None)
+    r"""OK"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/me.py` & `calendly-py-0.0.2/src/calendly/models/operations/me.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import user as shared_user
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class MeErrorResponseDetails:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_data_compliance_deletion_events.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_data_compliance_deletion_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostDataComplianceDeletionEventsRequestBody:
     r"""The start and end times that delineate the time range for scheduled events data deletion."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_data_compliance_deletion_invitees.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_data_compliance_deletion_invitees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostDataComplianceDeletionInviteesRequestBody:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_organizations_uuid_invitations.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_organizations_uuid_invitations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
 from ..shared import organizationinvitation as shared_organizationinvitation
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostOrganizationsUUIDInvitationsRequestBody:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_scheduled_events_uuid_cancellation.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_scheduled_events_uuid_cancellation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import cancellation as shared_cancellation
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostScheduledEventsUUIDCancellationApplicationJSON:
     r"""Optional cancellation reason."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_scheduling_links.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_scheduling_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class PostSchedulingLinksRequestBodyMaxEventCountEnum(str, Enum):
     r"""The max number of events that can be scheduled using this scheduling link."""
     ONE = '1'
 
 class PostSchedulingLinksRequestBodyOwnerTypeEnum(str, Enum):
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_shares.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_shares.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import share as shared_share
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostSharesRequestBodyAvailabilityRuleRulesIntervals:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/post_users_uuid_webhooks.py` & `calendly-py-0.0.2/src/calendly/models/operations/post_users_uuid_webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import webhooksubscription as shared_webhooksubscription
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 class PostUsersUUIDWebhooksRequestBodyEventsEnum(str, Enum):
     INVITEE_CANCELED = 'invitee.canceled'
     INVITEE_CREATED = 'invitee.created'
     ROUTING_FORM_SUBMISSION_CREATED = 'routing_form_submission.created'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/postinviteenoshow.py` & `calendly-py-0.0.2/src/calendly/models/operations/postinviteenoshow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import inviteenoshow as shared_inviteenoshow
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PostInviteeNoShowRequestBody:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/operations/revoke_users_organization_invitation.py` & `calendly-py-0.0.2/src/calendly/models/operations/revoke_users_organization_invitation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import errorresponse as shared_errorresponse
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclasses.dataclass
 class RevokeUsersOrganizationInvitationRequest:
     
     org_uuid: str = dataclasses.field(metadata={'path_param': { 'field_name': 'org_uuid', 'style': 'simple', 'explode': False }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/__init__.py` & `calendly-py-0.0.2/src/calendly/models/shared/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 from .organizationmembership import *
 from .outboundcall import *
 from .pagination import *
 from .profile import *
 from .question import *
 from .routingform import *
 from .routingformsubmission import *
+from .scheduledeventsresponse import *
 from .security import *
 from .share import *
 from .submissioncustommessageresult import *
 from .submissioneventtyperesult import *
 from .submissionexternalurlresult import *
 from .submissionquestionandanswer import *
 from .submissiontracking import *
 from .user import *
 from .userbusytime import *
 from .webexconference import *
 from .webhooksubscription import *
 from .zoomconference import *
 
-__all__ = ["Actor","ActorGroup","ActorOrganization","AvailabilityRule","AvailabilityRuleIntervals","AvailabilityRuleTypeEnum","AvailabilityRuleWdayEnum","AvailabilitySchedule","Cancellation","CancellationCancelerTypeEnum","CustomLocation","CustomLocationTypeEnum","Entry","ErrorResponse","ErrorResponseDetails","Event","EventEventMemberships","EventInviteesCounter","EventStatusEnum","EventType","EventTypeAvailableTime","EventTypeBookingMethodEnum","EventTypeCustomQuestion","EventTypeCustomQuestionTypeEnum","EventTypeKindDescriptionEnum","EventTypeKindEnum","EventTypePoolingTypeEnum","EventTypeTypeEnum","GoogleConference","GoogleConferenceStatusEnum","GoogleConferenceTypeEnum","GotoMeetingConference","GotoMeetingConferenceData","GotoMeetingConferenceStatusEnum","GotoMeetingConferenceTypeEnum","Guest","InPersonMeeting","InPersonMeetingTypeEnum","InboundCall","InboundCallTypeEnum","Invitee","InviteeNoShow","InviteeNoShow1","InviteePayment","InviteePaymentCurrencyEnum","InviteePaymentProviderEnum","InviteeQuestionAndAnswer","InviteeReconfirmation","InviteeSpecifiedLocation","InviteeSpecifiedLocationTypeEnum","InviteeStatusEnum","InviteeTracking","LegacyCalendarEvent","LegacyCalendarEventKindEnum","MicrosoftTeamsConference","MicrosoftTeamsConferenceData","MicrosoftTeamsConferenceDataAudioConferencing","MicrosoftTeamsConferenceStatusEnum","MicrosoftTeamsConferenceTypeEnum","OrganizationInvitation","OrganizationInvitationStatusEnum","OrganizationMembership","OrganizationMembershipRoleEnum","OrganizationMembershipUser","OutboundCall","OutboundCallTypeEnum","Pagination","Profile","ProfileTypeEnum","Question","QuestionTypeEnum","RoutingForm","RoutingFormStatusEnum","RoutingFormSubmission","RoutingFormSubmissionSubmitterTypeEnum","Security","Share","ShareSchedulingLinks","ShareSchedulingLinksOwnerTypeEnum","ShareShareOverride","ShareShareOverrideAvailabilityRule","ShareShareOverrideAvailabilityRuleRules","ShareShareOverrideAvailabilityRuleRulesIntervals","ShareShareOverrideAvailabilityRuleRulesTypeEnum","ShareShareOverrideAvailabilityRuleRulesWdayEnum","ShareShareOverrideLocationConfigurations","ShareShareOverrideLocationConfigurationsKindEnum","ShareShareOverridePeriodTypeEnum","SubmissionCustomMessageResult","SubmissionCustomMessageResultTypeEnum","SubmissionCustomMessageResultValue","SubmissionEventTypeResult","SubmissionEventTypeResultTypeEnum","SubmissionExternalURLResult","SubmissionExternalURLResultTypeEnum","SubmissionQuestionAndAnswer","SubmissionTracking","User","UserBusyTime","UserBusyTimeEvent","UserBusyTimeTypeEnum","WebExConference","WebExConferenceData","WebExConferenceDataTelephony","WebExConferenceDataTelephonyCallInNumbers","WebExConferenceStatusEnum","WebExConferenceTypeEnum","WebhookSubscription","WebhookSubscriptionEventsEnum","WebhookSubscriptionScopeEnum","WebhookSubscriptionStateEnum","ZoomConference","ZoomConferenceData","ZoomConferenceDataExtra","ZoomConferenceDataSettings","ZoomConferenceDataSettingsGlobalDialInNumbers","ZoomConferenceStatusEnum","ZoomConferenceTypeEnum"]
+__all__ = ["Actor","ActorGroup","ActorOrganization","AvailabilityRule","AvailabilityRuleIntervals","AvailabilityRuleTypeEnum","AvailabilityRuleWdayEnum","AvailabilitySchedule","Cancellation","CancellationCancelerTypeEnum","CustomLocation","CustomLocationTypeEnum","Entry","ErrorResponse","ErrorResponseDetails","Event","EventEventMemberships","EventInviteesCounter","EventStatusEnum","EventType","EventTypeAvailableTime","EventTypeBookingMethodEnum","EventTypeCustomQuestion","EventTypeCustomQuestionTypeEnum","EventTypeKindDescriptionEnum","EventTypeKindEnum","EventTypePoolingTypeEnum","EventTypeTypeEnum","GoogleConference","GoogleConferenceStatusEnum","GoogleConferenceTypeEnum","GotoMeetingConference","GotoMeetingConferenceData","GotoMeetingConferenceStatusEnum","GotoMeetingConferenceTypeEnum","Guest","InPersonMeeting","InPersonMeetingTypeEnum","InboundCall","InboundCallTypeEnum","Invitee","InviteeNoShow","InviteeNoShow1","InviteePayment","InviteePaymentCurrencyEnum","InviteePaymentProviderEnum","InviteeQuestionAndAnswer","InviteeReconfirmation","InviteeSpecifiedLocation","InviteeSpecifiedLocationTypeEnum","InviteeStatusEnum","InviteeTracking","LegacyCalendarEvent","LegacyCalendarEventKindEnum","MicrosoftTeamsConference","MicrosoftTeamsConferenceData","MicrosoftTeamsConferenceDataAudioConferencing","MicrosoftTeamsConferenceStatusEnum","MicrosoftTeamsConferenceTypeEnum","OrganizationInvitation","OrganizationInvitationStatusEnum","OrganizationMembership","OrganizationMembershipRoleEnum","OrganizationMembershipUser","OutboundCall","OutboundCallTypeEnum","Pagination","Profile","ProfileTypeEnum","Question","QuestionTypeEnum","RoutingForm","RoutingFormStatusEnum","RoutingFormSubmission","RoutingFormSubmissionSubmitterTypeEnum","ScheduledEventsResponse","Security","Share","ShareSchedulingLinks","ShareSchedulingLinksOwnerTypeEnum","ShareShareOverride","ShareShareOverrideAvailabilityRule","ShareShareOverrideAvailabilityRuleRules","ShareShareOverrideAvailabilityRuleRulesIntervals","ShareShareOverrideAvailabilityRuleRulesTypeEnum","ShareShareOverrideAvailabilityRuleRulesWdayEnum","ShareShareOverrideLocationConfigurations","ShareShareOverrideLocationConfigurationsKindEnum","ShareShareOverridePeriodTypeEnum","SubmissionCustomMessageResult","SubmissionCustomMessageResultTypeEnum","SubmissionCustomMessageResultValue","SubmissionEventTypeResult","SubmissionEventTypeResultTypeEnum","SubmissionExternalURLResult","SubmissionExternalURLResultTypeEnum","SubmissionQuestionAndAnswer","SubmissionTracking","User","UserBusyTime","UserBusyTimeEvent","UserBusyTimeTypeEnum","WebExConference","WebExConferenceData","WebExConferenceDataTelephony","WebExConferenceDataTelephonyCallInNumbers","WebExConferenceStatusEnum","WebExConferenceTypeEnum","WebhookSubscription","WebhookSubscriptionEventsEnum","WebhookSubscriptionScopeEnum","WebhookSubscriptionStateEnum","ZoomConference","ZoomConferenceData","ZoomConferenceDataExtra","ZoomConferenceDataSettings","ZoomConferenceDataSettingsGlobalDialInNumbers","ZoomConferenceStatusEnum","ZoomConferenceTypeEnum"]
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/actor.py` & `calendly-py-0.0.2/src/calendly/models/shared/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ActorGroup:
     r"""User group information about the actor"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/availabilityrule.py` & `calendly-py-0.0.2/src/calendly/models/shared/availabilityrule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AvailabilityRuleIntervals:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/availabilityschedule.py` & `calendly-py-0.0.2/src/calendly/models/shared/availabilityschedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from ..shared import availabilityrule as shared_availabilityrule
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class AvailabilitySchedule:
     r"""The availability schedule set by the user."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/cancellation.py` & `calendly-py-0.0.2/src/calendly/models/shared/cancellation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class CancellationCancelerTypeEnum(str, Enum):
     HOST = 'host'
     INVITEE = 'invitee'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/customlocation.py` & `calendly-py-0.0.2/src/calendly/models/shared/customlocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class CustomLocationTypeEnum(str, Enum):
     r"""The event location doesn't fall into a standard category defined by the event host (publisher)"""
     CUSTOM = 'custom'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/entry.py` & `calendly-py-0.0.2/src/calendly/models/shared/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import actor as shared_actor
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Entry:
     r"""Object for a created activity log record"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/errorresponse.py` & `calendly-py-0.0.2/src/calendly/models/shared/errorresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ErrorResponseDetails:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/event.py` & `calendly-py-0.0.2/src/calendly/models/shared/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import cancellation as shared_cancellation
 from ..shared import guest as shared_guest
 from ..shared import legacycalendarevent as shared_legacycalendarevent
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EventEventMemberships:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/eventtype.py` & `calendly-py-0.0.2/src/calendly/models/shared/eventtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import eventtypecustomquestion as shared_eventtypecustomquestion
 from ..shared import profile as shared_profile
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 
 class EventTypeBookingMethodEnum(str, Enum):
     r"""Indicates if the event type is for a poll or an instant booking"""
     INSTANT = 'instant'
     POLL = 'poll'
 
 class EventTypeKindEnum(str, Enum):
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/eventtypeavailabletime.py` & `calendly-py-0.0.2/src/calendly/models/shared/eventtypeavailabletime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class EventTypeAvailableTime:
     r"""An available meeting time slot for the given event type"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/eventtypecustomquestion.py` & `calendly-py-0.0.2/src/calendly/models/shared/eventtypecustomquestion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class EventTypeCustomQuestionTypeEnum(str, Enum):
     r"""The type of response that the invitee provides to the custom question; can be one or multiple lines of text, a phone number, or single- or multiple-select."""
     STRING = 'string'
     TEXT = 'text'
     PHONE_NUMBER = 'phone_number'
     SINGLE_SELECT = 'single_select'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/googleconference.py` & `calendly-py-0.0.2/src/calendly/models/shared/googleconference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class GoogleConferenceStatusEnum(str, Enum):
     r"""Indicates the current status of the Google conference"""
     INITIATED = 'initiated'
     PROCESSING = 'processing'
     PUSHED = 'pushed'
     FAILED = 'failed'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/gotomeetingconference.py` & `calendly-py-0.0.2/src/calendly/models/shared/gotomeetingconference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GotoMeetingConferenceData:
     r"""The conference metadata supplied by GoToMeeting"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/guest.py` & `calendly-py-0.0.2/src/calendly/models/shared/guest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Guest:
     r"""An individual whom an invitee has invited to be a guest attendee to an event"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inboundcall.py` & `calendly-py-0.0.2/src/calendly/models/shared/submissioneventtyperesult.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
-class InboundCallTypeEnum(str, Enum):
-    r"""Indicates that the invitee will call the event host"""
-    INBOUND_CALL = 'inbound_call'
+class SubmissionEventTypeResultTypeEnum(str, Enum):
+    r"""Indicates that the routing form submission resulted in a redirect to an event type booking page."""
+    EVENT_TYPE = 'event_type'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class InboundCall:
-    r"""Invitee will call meeting publisher at the specified phone number"""
+class SubmissionEventTypeResult:
+    r"""Information about the event type Routing Form Submission result."""
     
-    location: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
-    r"""The phone number the invitee will use to call the event host (publisher)"""  
-    type: InboundCallTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""Indicates that the invitee will call the event host"""  
+    type: SubmissionEventTypeResultTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""Indicates that the routing form submission resulted in a redirect to an event type booking page."""  
+    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
+    r"""A reference to the event type resource."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inpersonmeeting.py` & `calendly-py-0.0.2/src/calendly/models/shared/inpersonmeeting.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class InPersonMeetingTypeEnum(str, Enum):
     r"""Indicates that the event will be an in-person meeting."""
     PHYSICAL = 'physical'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/invitee.py` & `calendly-py-0.0.2/src/calendly/models/shared/invitee.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import cancellation as shared_cancellation
 from ..shared import inviteequestionandanswer as shared_inviteequestionandanswer
 from ..shared import inviteetracking as shared_inviteetracking
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InviteeNoShow1:
     r"""Provides data pertaining to the associated no show for the Invitee"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inviteenoshow.py` & `calendly-py-0.0.2/src/calendly/models/shared/inviteenoshow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InviteeNoShow:
     r"""Information about an invitees no show."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inviteequestionandanswer.py` & `calendly-py-0.0.2/src/calendly/models/shared/inviteequestionandanswer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InviteeQuestionAndAnswer:
     r"""A response to a question on a booking page form"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inviteespecifiedlocation.py` & `calendly-py-0.0.2/src/calendly/models/shared/inviteespecifiedlocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class InviteeSpecifiedLocationTypeEnum(str, Enum):
     r"""The event location selected by the invitee"""
     ASK_INVITEE = 'ask_invitee'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/inviteetracking.py` & `calendly-py-0.0.2/src/calendly/models/shared/inviteetracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InviteeTracking:
     r"""The UTM and Salesforce tracking parameters associated with an Invitee"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/legacycalendarevent.py` & `calendly-py-0.0.2/src/calendly/models/shared/legacycalendarevent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class LegacyCalendarEventKindEnum(str, Enum):
     r"""Indicates the calendar provider the event belongs to."""
     EXCHANGE = 'exchange'
     GOOGLE = 'google'
     ICLOUD = 'icloud'
     OUTLOOK = 'outlook'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/microsoftteamsconference.py` & `calendly-py-0.0.2/src/calendly/models/shared/microsoftteamsconference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class MicrosoftTeamsConferenceDataAudioConferencing:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/organizationinvitation.py` & `calendly-py-0.0.2/src/calendly/models/shared/organizationinvitation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 class OrganizationInvitationStatusEnum(str, Enum):
     r"""The status of the invitation (\\"pending\\", \\"accepted\\", or \\"declined\\")"""
     PENDING = 'pending'
     ACCEPTED = 'accepted'
     DECLINED = 'declined'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/organizationmembership.py` & `calendly-py-0.0.2/src/calendly/models/shared/organizationmembership.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 
 class OrganizationMembershipRoleEnum(str, Enum):
     r"""The user's role in the organization"""
     USER = 'user'
     ADMIN = 'admin'
     OWNER = 'owner'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/outboundcall.py` & `calendly-py-0.0.2/src/calendly/models/shared/inboundcall.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
-class OutboundCallTypeEnum(str, Enum):
-    r"""Indicates that the event host (publisher) will call the invitee"""
-    OUTBOUND_CALL = 'outbound_call'
+class InboundCallTypeEnum(str, Enum):
+    r"""Indicates that the invitee will call the event host"""
+    INBOUND_CALL = 'inbound_call'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class OutboundCall:
-    r"""Meeting publisher will call the Invitee"""
+class InboundCall:
+    r"""Invitee will call meeting publisher at the specified phone number"""
     
     location: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
-    r"""The phone number the event host (publisher) will use to call the invitee"""  
-    type: OutboundCallTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""Indicates that the event host (publisher) will call the invitee"""  
+    r"""The phone number the invitee will use to call the event host (publisher)"""  
+    type: InboundCallTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""Indicates that the invitee will call the event host"""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/pagination.py` & `calendly-py-0.0.2/src/calendly/models/shared/pagination.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Pagination:
     
     count: float = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('count') }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/profile.py` & `calendly-py-0.0.2/src/calendly/models/shared/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class ProfileTypeEnum(str, Enum):
     r"""Indicates if the profile belongs to a \\"user\\" (individual) or \\"team\\" """
     USER = 'User'
     TEAM = 'Team'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/question.py` & `calendly-py-0.0.2/src/calendly/models/shared/question.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class QuestionTypeEnum(str, Enum):
     r"""Question type: name, text input, email, phone, textarea input, dropdown list or radio button list."""
     NAME = 'name'
     TEXT = 'text'
     EMAIL = 'email'
     PHONE = 'phone'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/routingform.py` & `calendly-py-0.0.2/src/calendly/models/shared/routingform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import question as shared_question
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 
 class RoutingFormStatusEnum(str, Enum):
     r"""Indicates if the form is in \\"draft\\" or \\"published\\" status."""
     DRAFT = 'draft'
     PUBLISHED = 'published'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/routingformsubmission.py` & `calendly-py-0.0.2/src/calendly/models/shared/routingformsubmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from ..shared import submissionquestionandanswer as shared_submissionquestionandanswer
 from ..shared import submissiontracking as shared_submissiontracking
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Any, Optional
 
 class RoutingFormSubmissionSubmitterTypeEnum(str, Enum):
     r"""Type of the respondent resource that submitted the form and scheduled a meeting."""
     INVITEE = 'Invitee'
     NULL = 'null'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/security.py` & `calendly-py-0.0.2/src/calendly/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/share.py` & `calendly-py-0.0.2/src/calendly/models/shared/share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 class ShareSchedulingLinksOwnerTypeEnum(str, Enum):
     r"""Resource type (currently, this is always EventType)"""
     EVENT_TYPE = 'EventType'
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/submissioncustommessageresult.py` & `calendly-py-0.0.2/src/calendly/models/shared/submissioncustommessageresult.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 class SubmissionCustomMessageResultTypeEnum(str, Enum):
     r"""Indicates if the routing form submission resulted in a custom \\"thank you\\" message."""
     CUSTOM_MESSAGE = 'custom_message'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/submissioneventtyperesult.py` & `calendly-py-0.0.2/src/calendly/models/shared/submissionexternalurlresult.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
-class SubmissionEventTypeResultTypeEnum(str, Enum):
-    r"""Indicates that the routing form submission resulted in a redirect to an event type booking page."""
-    EVENT_TYPE = 'event_type'
+class SubmissionExternalURLResultTypeEnum(str, Enum):
+    r"""Indicates that the routing form submission resulted in a redirect to an external URL."""
+    EXTERNAL_URL = 'external_url'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SubmissionEventTypeResult:
-    r"""Information about the event type Routing Form Submission result."""
+class SubmissionExternalURLResult:
+    r"""Information about the external URL Routing Form Submission result."""
     
-    type: SubmissionEventTypeResultTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""Indicates that the routing form submission resulted in a redirect to an event type booking page."""  
+    type: SubmissionExternalURLResultTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
+    r"""Indicates that the routing form submission resulted in a redirect to an external URL."""  
     value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    r"""A reference to the event type resource."""  
+    r"""The external URL the respondent were redirected to."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/submissionexternalurlresult.py` & `calendly-py-0.0.2/src/calendly/models/shared/scheduledeventsresponse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import event as shared_event
+from ..shared import pagination as shared_pagination
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-from sdk import utils
-
-class SubmissionExternalURLResultTypeEnum(str, Enum):
-    r"""Indicates that the routing form submission resulted in a redirect to an external URL."""
-    EXTERNAL_URL = 'external_url'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SubmissionExternalURLResult:
-    r"""Information about the external URL Routing Form Submission result."""
+class ScheduledEventsResponse:
+    r"""Service response"""
     
-    type: SubmissionExternalURLResultTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""Indicates that the routing form submission resulted in a redirect to an external URL."""  
-    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
-    r"""The external URL the respondent were redirected to."""  
+    collection: list[shared_event.Event] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('collection') }})
+    r"""The set of scheduled events matching the criteria"""  
+    pagination: shared_pagination.Pagination = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pagination') }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/submissionquestionandanswer.py` & `calendly-py-0.0.2/src/calendly/models/shared/submissionquestionandanswer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SubmissionQuestionAndAnswer:
     r"""All Routing Form Submission questions with answers."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/submissiontracking.py` & `calendly-py-0.0.2/src/calendly/models/shared/submissiontracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SubmissionTracking:
     r"""The UTM and Salesforce tracking parameters associated with a Routing Form Submission."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/user.py` & `calendly-py-0.0.2/src/calendly/models/shared/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from marshmallow import fields
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class User:
     r"""Information about the user."""
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/userbusytime.py` & `calendly-py-0.0.2/src/calendly/models/shared/userbusytime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserBusyTimeEvent:
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/webexconference.py` & `calendly-py-0.0.2/src/calendly/models/shared/webexconference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WebExConferenceDataTelephonyCallInNumbers:
     
     call_in_number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('callInNumber') }})
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/webhooksubscription.py` & `calendly-py-0.0.2/src/calendly/models/shared/webhooksubscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from sdk import utils
 
 class WebhookSubscriptionEventsEnum(str, Enum):
     INVITEE_CREATED = 'invitee.created'
     INVITEE_CANCELED = 'invitee.canceled'
     ROUTING_FORM_SUBMISSION_CREATED = 'routing_form_submission.created'
 
 class WebhookSubscriptionScopeEnum(str, Enum):
```

### Comparing `calendly-py-0.0.1/src/sdk/models/shared/zoomconference.py` & `calendly-py-0.0.2/src/calendly/models/shared/zoomconference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from calendly import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
-from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ZoomConferenceDataExtra:
```

### Comparing `calendly-py-0.0.1/src/sdk/organizations.py` & `calendly-py-0.0.2/src/calendly/organizations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations, shared
+from calendly.models import operations, shared
 from typing import Optional
 
 class Organizations:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/routing_forms.py` & `calendly-py-0.0.2/src/calendly/routing_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class RoutingForms:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/scheduled_events.py` & `calendly-py-0.0.2/src/calendly/scheduled_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations, shared
+from calendly.models import operations, shared
 from typing import Optional
 
 class ScheduledEvents:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
@@ -233,16 +233,16 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListScheduledEventsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListScheduledEvents200ApplicationJSON])
-                res.list_scheduled_events_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ScheduledEventsResponse])
+                res.scheduled_events_response = out
         elif http_res.status_code in [400, 401, 404, 500]:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.ListScheduledEventsErrorResponse])
                 res.error_response = out
         elif http_res.status_code == 403:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[operations.ListScheduledEvents403ApplicationJSON])
```

### Comparing `calendly-py-0.0.1/src/sdk/scheduling_links.py` & `calendly-py-0.0.2/src/calendly/scheduling_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class SchedulingLinks:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/sdk.py` & `calendly-py-0.0.2/src/calendly/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 from .organizations import Organizations
 from .routing_forms import RoutingForms
 from .scheduled_events import ScheduledEvents
 from .scheduling_links import SchedulingLinks
 from .shares import Shares
 from .users import Users
 from .webhooks import Webhooks
-from sdk.models import shared
+from calendly.models import shared
 
 SERVERS = [
     "https://api.calendly.com",
 ]
 """Contains the list of servers available to the SDK"""
 
-class SDK:
+class Calendly:
     r"""Calendly’s API is [REST](http://en.wikipedia.org/wiki/Representational_State_Transfer)-based and has predictable resource-oriented URLs. It uses **JSON** for request and response bodies and standard HTTP methods, authentication, and response codes.<br>
     
     ##### Authenticate with personal access tokens or OAuth 2.0
     
     To access Calendly data through the API, you can authenticate with **personal access tokens** or **OAuth 2.0**. To learn more about these authentication methods and when and how to use them, see [Getting Started with the Calendly API](https://developer.calendly.com/getting-started).
     """
     activity_log: ActivityLog
@@ -39,15 +39,15 @@
     users: Users
     webhooks: Webhooks
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.0.1"
+    _sdk_version: str = "0.0.2"
     _gen_version: str = "2.17.8"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
```

### Comparing `calendly-py-0.0.1/src/sdk/shares.py` & `calendly-py-0.0.2/src/calendly/shares.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class Shares:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/users.py` & `calendly-py-0.0.2/src/calendly/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations, shared
+from calendly.models import operations, shared
 from typing import Optional
 
 class Users:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

### Comparing `calendly-py-0.0.1/src/sdk/utils/retries.py` & `calendly-py-0.0.2/src/calendly/utils/retries.py`

 * *Files identical despite different names*

### Comparing `calendly-py-0.0.1/src/sdk/utils/utils.py` & `calendly-py-0.0.2/src/calendly/utils/utils.py`

 * *Files identical despite different names*

### Comparing `calendly-py-0.0.1/src/sdk/webhooks.py` & `calendly-py-0.0.2/src/calendly/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from sdk.models import operations
+from calendly.models import operations
 from typing import Optional
 
 class Webhooks:
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
```

