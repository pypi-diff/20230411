# Comparing `tmp/stigg-api-client-0.2.0.tar.gz` & `tmp/stigg-api-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg-api-client-0.2.0.tar", max compression
+gzip compressed data, was "stigg-api-client-0.3.0.tar", max compression
```

## Comparing `stigg-api-client-0.2.0.tar` & `stigg-api-client-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg-api-client-0.2.0/README.md
--rw-r--r--   0        0        0      396 2023-04-02 10:54:59.841923 stigg-api-client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-03-05 12:25:06.527501 stigg-api-client-0.2.0/stigg/__init__.py
--rw-r--r--   0        0        0      997 2023-03-05 12:25:06.527623 stigg-api-client-0.2.0/stigg/client.py
--rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg-api-client-0.2.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0    44087 2023-04-02 10:54:35.882732 stigg-api-client-0.2.0/stigg/generated/operations.py
--rw-r--r--   0        0        0   430709 2023-04-02 10:54:35.619739 stigg-api-client-0.2.0/stigg/generated/schema.py
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 stigg-api-client-0.2.0/setup.py
--rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 stigg-api-client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2479 2023-03-05 12:25:06.526402 stigg-api-client-0.3.0/README.md
+-rw-r--r--   0        0        0      396 2023-04-11 10:26:38.527477 stigg-api-client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-03-05 12:25:06.527501 stigg-api-client-0.3.0/stigg/__init__.py
+-rw-r--r--   0        0        0      997 2023-03-05 12:25:06.527623 stigg-api-client-0.3.0/stigg/client.py
+-rw-r--r--   0        0        0        0 2023-03-05 12:25:06.527730 stigg-api-client-0.3.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0    43935 2023-04-11 10:24:57.366059 stigg-api-client-0.3.0/stigg/generated/operations.py
+-rw-r--r--   0        0        0   432273 2023-04-11 10:24:57.216151 stigg-api-client-0.3.0/stigg/generated/schema.py
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 stigg-api-client-0.3.0/setup.py
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 stigg-api-client-0.3.0/PKG-INFO
```

### Comparing `stigg-api-client-0.2.0/README.md` & `stigg-api-client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg-api-client-0.2.0/stigg/client.py` & `stigg-api-client-0.3.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg-api-client-0.2.0/stigg/generated/operations.py` & `stigg-api-client-0.3.0/stigg/generated/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,15 @@
     return _frag
 
 
 def fragment_customer_fragment():
     _frag = sgqlc.operation.Fragment(_schema.Customer, 'CustomerFragment')
     _frag.__fragment__(fragment_slim_customer_fragment())
     _frag.has_payment_method()
+    _frag.has_active_subscription()
     _frag.default_payment_expiration_month()
     _frag.default_payment_expiration_year()
     _frag.default_payment_method_last4_digits()
     _frag_trialed_plans = _frag.trialed_plans()
     _frag_trialed_plans.product_id()
     _frag_trialed_plans.product_ref_id()
     _frag_trialed_plans.plan_ref_id()
@@ -344,29 +345,17 @@
     return _frag
 
 
 def fragment_reset_period_configuration_fragment():
     _frag = sgqlc.operation.Fragment(_schema.ResetPeriodConfiguration, 'ResetPeriodConfigurationFragment')
     _frag.__typename__()
     _frag__as__MonthlyResetPeriodConfig = _frag.__as__(_schema.MonthlyResetPeriodConfig)
-    _frag__as__MonthlyResetPeriodConfig.__fragment__(fragment_monthly_reset_period_config_fragment())
+    _frag__as__MonthlyResetPeriodConfig.monthly_according_to()
     _frag__as__WeeklyResetPeriodConfig = _frag.__as__(_schema.WeeklyResetPeriodConfig)
-    _frag__as__WeeklyResetPeriodConfig.__fragment__(fragment_weekly_reset_period_config_fragment())
-    return _frag
-
-
-def fragment_monthly_reset_period_config_fragment():
-    _frag = sgqlc.operation.Fragment(_schema.MonthlyResetPeriodConfig, 'MonthlyResetPeriodConfigFragment')
-    _frag.monthly_according_to()
-    return _frag
-
-
-def fragment_weekly_reset_period_config_fragment():
-    _frag = sgqlc.operation.Fragment(_schema.WeeklyResetPeriodConfig, 'WeeklyResetPeriodConfigFragment')
-    _frag.weekly_according_to()
+    _frag__as__WeeklyResetPeriodConfig.weekly_according_to()
     return _frag
 
 
 def fragment_usage_updated_fragment():
     _frag = sgqlc.operation.Fragment(_schema.UsageMeasurementUpdated, 'UsageUpdatedFragment')
     _frag.customer_id()
     _frag.resource_id()
@@ -803,15 +792,14 @@
     feature_fragment = fragment_feature_fragment()
     font_variant_fragment = fragment_font_variant_fragment()
     layout_configuration_fragment = fragment_layout_configuration_fragment()
     mock_paywall_addon_fragment = fragment_mock_paywall_addon_fragment()
     mock_paywall_package_entitlement_fragment = fragment_mock_paywall_package_entitlement_fragment()
     mock_paywall_plan_fragment = fragment_mock_paywall_plan_fragment()
     mock_paywall_price_fragment = fragment_mock_paywall_price_fragment()
-    monthly_reset_period_config_fragment = fragment_monthly_reset_period_config_fragment()
     package_entitlement_fragment = fragment_package_entitlement_fragment()
     paywall_addon_fragment = fragment_paywall_addon_fragment()
     paywall_configuration_fragment = fragment_paywall_configuration_fragment()
     paywall_currency = fragment_paywall_currency()
     paywall_fragment = fragment_paywall_fragment()
     paywall_package_entitlement_fragment = fragment_paywall_package_entitlement_fragment()
     paywall_plan_fragment = fragment_paywall_plan_fragment()
@@ -824,15 +812,14 @@
     slim_subscription_fragment = fragment_slim_subscription_fragment()
     subscription_fragment = fragment_subscription_fragment()
     subscription_preview_fragment = fragment_subscription_preview_fragment()
     subscription_scheduled_update_data = fragment_subscription_scheduled_update_data()
     total_price_fragment = fragment_total_price_fragment()
     typography_configuration_fragment = fragment_typography_configuration_fragment()
     usage_updated_fragment = fragment_usage_updated_fragment()
-    weekly_reset_period_config_fragment = fragment_weekly_reset_period_config_fragment()
 
 
 def mutation_provision_customer():
     _op = sgqlc.operation.Operation(_schema_root.mutation_type, name='ProvisionCustomer', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.ProvisionCustomerInput))))
     _op_provision_customer = _op.provision_customer(input=sgqlc.types.Variable('input'))
     _op_provision_customer_customer = _op_provision_customer.customer()
     _op_provision_customer_customer.__fragment__(fragment_slim_customer_fragment())
@@ -950,14 +937,21 @@
 def query_get_customer_by_id():
     _op = sgqlc.operation.Operation(_schema_root.query_type, name='GetCustomerById', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.GetCustomerByRefIdInput))))
     _op_get_customer_by_ref_id = _op.get_customer_by_ref_id(input=sgqlc.types.Variable('input'))
     _op_get_customer_by_ref_id.__fragment__(fragment_customer_fragment())
     return _op
 
 
+def query_get_active_subscriptions():
+    _op = sgqlc.operation.Operation(_schema_root.query_type, name='GetActiveSubscriptions', variables=dict(input=sgqlc.types.Arg(sgqlc.types.non_null(_schema.GetActiveSubscriptionsInput))))
+    _op_get_active_subscriptions = _op.get_active_subscriptions(input=sgqlc.types.Variable('input'))
+    _op_get_active_subscriptions.__fragment__(fragment_subscription_fragment())
+    return _op
+
+
 def query_get_coupons():
     _op = sgqlc.operation.Operation(_schema_root.query_type, name='GetCoupons')
     _op_coupons = _op.coupons(filter={'status': {'eq': 'ACTIVE'}}, paging={'first': 50})
     _op_coupons_edges = _op_coupons.edges()
     _op_coupons_edges_node = _op_coupons_edges.node()
     _op_coupons_edges_node.__fragment__(fragment_coupon_fragment())
     return _op
@@ -1015,14 +1009,15 @@
     _op_mock_paywall_plans.__fragment__(fragment_mock_paywall_plan_fragment())
     _op_mock_paywall_configuration = _op_mock_paywall.configuration()
     _op_mock_paywall_configuration.__fragment__(fragment_paywall_configuration_fragment())
     return _op
 
 
 class Query:
+    get_active_subscriptions = query_get_active_subscriptions()
     get_coupons = query_get_coupons()
     get_customer_by_id = query_get_customer_by_id()
     get_customer_portal_by_ref_id = query_get_customer_portal_by_ref_id()
     get_entitlement = query_get_entitlement()
     get_entitlements = query_get_entitlements()
     get_mock_paywall = query_get_mock_paywall()
     get_paywall = query_get_paywall()
```

### Comparing `stigg-api-client-0.2.0/stigg/generated/schema.py` & `stigg-api-client-0.3.0/stigg/generated/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 class ErrorCode(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('AccountNotFoundError', 'AddonHasToHavePriceError', 'AddonNotFound', 'ArchivedCouponCantBeApplied', 'AuthCustomerMismatch', 'BadUserInput', 'BillingPeriodMissingError', 'CannotDeleteCustomerError', 'CannotDeleteFeatureError', 'CannotEditPackageInNonDraftMode', 'CheckoutIsNotSupported', 'CheckoutOptionsMissing', 'CouponNotFound', 'CustomerAlreadyHaveCustomerCoupon', 'CustomerAlreadyUsesCoupon', 'CustomerHasNoPaymentMethod', 'CustomerNoBillingId', 'CustomerNotFound', 'CustomerResourceNotFound', 'DowngradeBillingPeriodNotSupportedError', 'DraftPlanCantBeArchived', 'DuplicatedEntityNotAllowed', 'EditAllowedOnDraftPackageOnlyError', 'EntitlementsMustBelongToSamePackage', 'EntityIdDifferentFromRefIdError', 'EnvironmentMissing', 'ExperimentAlreadyRunning', 'ExperimentNotFoundError', 'ExperimentStatusError', 'FailedToCreateCheckoutSessionError', 'FailedToImportCustomer', 'FeatureNotFound', 'FetchAllCountriesPricesNotAllowed', 'IdentityForbidden', 'ImportAlreadyInProgress', 'InitStripePaymentMethodError', 'IntegrationNotFound', 'IntegrityViolation', 'InvalidAddressError', 'InvalidArgumentError', 'InvalidCancellationDate', 'InvalidEntitlementResetPeriod', 'InvalidMemberDelete', 'InvalidQuantity', 'InvalidSubscriptionStatus', 'InvalidUpdatePriceUnitAmountError', 'InvalidUsageValueForIncrementalFeatureError', 'MemberInvitationError', 'MemberNotFound', 'MeteringNotAvailableForFeatureType', 'MissingEntityIdError', 'NoFeatureEntitlementInSubscription', 'NoProductsAvailable', 'OperationNotAllowedDuringInProgressExperiment', 'PackageAlreadyPublished', 'PackagePricingTypeNotSet', 'PlanAlreadyExtended', 'PlanCannotBePublishWhenBasePlanIsDraft', 'PlanIsUsedAsDefaultStartPlan', 'PlanIsUsedAsDowngradePlan', 'PlanNotFound', 'PlanWithChildCantBeDeleted', 'PlansCircularDependencyError', 'PriceNotFound', 'PromotionCodeCustomerNotFirstPurchase', 'PromotionCodeMaxRedemptionsReached', 'PromotionCodeMinimumAmountNotReached', 'PromotionCodeNotActive', 'PromotionCodeNotForCustomer', 'PromotionCodeNotFound', 'RateLimitExceeded', 'ResyncAlreadyInProgress', 'SelectedBillingModelDoesntMatchImportedItemError', 'StripeCustomerIsDeleted', 'SubscriptionAlreadyCanceledOrExpired', 'SubscriptionMustHaveSinglePlanError', 'SubscriptionNotFound', 'TrialMinDateError', 'TrialMustBeCancelledImmediately', 'UnPublishedPackage', 'Unauthenticated', 'UncompatibleSubscriptionAddon', 'UnexpectedError', 'UnsupportedFeatureType', 'UnsupportedSubscriptionScheduleType', 'UnsupportedVendorIdentifier')
 
 
 class EventLogType(sgqlc.types.Enum):
     __schema__ = schema
-    __choices__ = ('ADDON_CREATED', 'ADDON_DELETED', 'ADDON_UPDATED', 'COUPON_ARCHIVED', 'COUPON_CREATED', 'COUPON_UPDATED', 'CREATE_SUBSCRIPTION_FAILED', 'CUSTOMER_CREATED', 'CUSTOMER_DELETED', 'CUSTOMER_PAYMENT_FAILED', 'CUSTOMER_UPDATED', 'EDGE_API_DATA_RESYNC', 'ENTITLEMENTS_UPDATED', 'ENTITLEMENT_DENIED', 'ENTITLEMENT_GRANTED', 'ENTITLEMENT_REQUESTED', 'ENVIRONMENT_DELETED', 'FEATURE_CREATED', 'FEATURE_DELETED', 'FEATURE_UPDATED', 'IMPORT_INTEGRATION_CATALOG_TRIGGERED', 'IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED', 'MEASUREMENT_REPORTED', 'PACKAGE_PUBLISHED', 'PLAN_CREATED', 'PLAN_DELETED', 'PLAN_UPDATED', 'PRODUCT_CREATED', 'PRODUCT_DELETED', 'PRODUCT_UPDATED', 'PROMOTIONAL_ENTITLEMENT_EXPIRED', 'PROMOTIONAL_ENTITLEMENT_GRANTED', 'PROMOTIONAL_ENTITLEMENT_REVOKED', 'PROMOTIONAL_ENTITLEMENT_UPDATED', 'RESYNC_INTEGRATION_TRIGGERED', 'SUBSCRIPTION_CANCELED', 'SUBSCRIPTION_CREATED', 'SUBSCRIPTION_EXPIRED', 'SUBSCRIPTION_TRIAL_CONVERTED', 'SUBSCRIPTION_TRIAL_ENDS_SOON', 'SUBSCRIPTION_TRIAL_EXPIRED', 'SUBSCRIPTION_TRIAL_STARTED', 'SUBSCRIPTION_UPDATED', 'SUBSCRIPTION_USAGE_UPDATED', 'SYNC_FAILED', 'WIDGET_CONFIGURATION_UPDATED')
+    __choices__ = ('ADDON_CREATED', 'ADDON_DELETED', 'ADDON_UPDATED', 'COUPON_ARCHIVED', 'COUPON_CREATED', 'COUPON_UPDATED', 'CREATE_SUBSCRIPTION_FAILED', 'CUSTOMER_CREATED', 'CUSTOMER_DELETED', 'CUSTOMER_PAYMENT_FAILED', 'CUSTOMER_RESOURCE_ENTITLEMENT_CALCULATION_TRIGGERED', 'CUSTOMER_UPDATED', 'EDGE_API_DATA_RESYNC', 'ENTITLEMENTS_UPDATED', 'ENTITLEMENT_DENIED', 'ENTITLEMENT_GRANTED', 'ENTITLEMENT_REQUESTED', 'ENVIRONMENT_DELETED', 'FEATURE_CREATED', 'FEATURE_DELETED', 'FEATURE_UPDATED', 'IMPORT_INTEGRATION_CATALOG_TRIGGERED', 'IMPORT_INTEGRATION_CUSTOMERS_TRIGGERED', 'MEASUREMENT_REPORTED', 'PACKAGE_PUBLISHED', 'PLAN_CREATED', 'PLAN_DELETED', 'PLAN_UPDATED', 'PRODUCT_CREATED', 'PRODUCT_DELETED', 'PRODUCT_UPDATED', 'PROMOTIONAL_ENTITLEMENT_EXPIRED', 'PROMOTIONAL_ENTITLEMENT_GRANTED', 'PROMOTIONAL_ENTITLEMENT_REVOKED', 'PROMOTIONAL_ENTITLEMENT_UPDATED', 'RESYNC_INTEGRATION_TRIGGERED', 'SUBSCRIPTION_CANCELED', 'SUBSCRIPTION_CREATED', 'SUBSCRIPTION_EXPIRED', 'SUBSCRIPTION_TRIAL_CONVERTED', 'SUBSCRIPTION_TRIAL_ENDS_SOON', 'SUBSCRIPTION_TRIAL_EXPIRED', 'SUBSCRIPTION_TRIAL_STARTED', 'SUBSCRIPTION_UPDATED', 'SUBSCRIPTION_USAGE_UPDATED', 'SYNC_FAILED', 'WIDGET_CONFIGURATION_UPDATED')
 
 
 class ExperimentSortFields(sgqlc.types.Enum):
     __schema__ = schema
     __choices__ = ('createdAt', 'environmentId', 'id', 'name', 'productId', 'refId', 'status')
 
 
@@ -592,17 +592,18 @@
     collect_phone_number = sgqlc.types.Field(Boolean, graphql_name='collectPhoneNumber')
     reference_id = sgqlc.types.Field(String, graphql_name='referenceId')
     success_url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='successUrl')
 
 
 class ClearCustomerPersistentCacheInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('customer_id', 'environment_id')
+    __field_names__ = ('customer_id', 'environment_id', 'resource_id')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class CouponFilter(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('and_', 'billing_id', 'created_at', 'customers', 'description', 'environment_id', 'id', 'name', 'or_', 'ref_id', 'status', 'type', 'updated_at')
     and_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('CouponFilter')), graphql_name='and')
     billing_id = sgqlc.types.Field('StringFieldComparison', graphql_name='billingId')
@@ -694,15 +695,16 @@
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     ref_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='refId')
     type = sgqlc.types.Field(sgqlc.types.non_null(CouponType), graphql_name='type')
 
 
 class CreateEnvironment(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'provision_status', 'slug')
+    __field_names__ = ('color', 'created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'provision_status', 'slug')
+    color = sgqlc.types.Field(String, graphql_name='color')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(String, graphql_name='displayName')
     harden_client_access_enabled = sgqlc.types.Field(Boolean, graphql_name='hardenClientAccessEnabled')
     id = sgqlc.types.Field(String, graphql_name='id')
     provision_status = sgqlc.types.Field(EnvironmentProvisionStatus, graphql_name='provisionStatus')
     slug = sgqlc.types.Field(String, graphql_name='slug')
@@ -1156,15 +1158,16 @@
     id = sgqlc.types.Field('StringFieldComparison', graphql_name='id')
     or_ = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('EnvironmentFilter')), graphql_name='or')
     slug = sgqlc.types.Field('StringFieldComparison', graphql_name='slug')
 
 
 class EnvironmentInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('description', 'display_name', 'harden_client_access_enabled', 'provision_status')
+    __field_names__ = ('color', 'description', 'display_name', 'harden_client_access_enabled', 'provision_status')
+    color = sgqlc.types.Field(String, graphql_name='color')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(String, graphql_name='displayName')
     harden_client_access_enabled = sgqlc.types.Field(Boolean, graphql_name='hardenClientAccessEnabled')
     provision_status = sgqlc.types.Field(EnvironmentProvisionStatus, graphql_name='provisionStatus')
 
 
 class EnvironmentSort(sgqlc.types.Input):
@@ -1369,14 +1372,22 @@
 class FontVariantInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('font_size', 'font_weight')
     font_size = sgqlc.types.Field(Float, graphql_name='fontSize')
     font_weight = sgqlc.types.Field(FontWeight, graphql_name='fontWeight')
 
 
+class GetActiveSubscriptionsInput(sgqlc.types.Input):
+    __schema__ = schema
+    __field_names__ = ('customer_id', 'environment_id', 'resource_id')
+    customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
+    environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
+    resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
+
+
 class GetCustomerByRefIdInput(sgqlc.types.Input):
     __schema__ = schema
     __field_names__ = ('customer_id', 'environment_id')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     environment_id = sgqlc.types.Field(String, graphql_name='environmentId')
 
 
@@ -2148,19 +2159,20 @@
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     should_sync_free = sgqlc.types.Field(Boolean, graphql_name='shouldSyncFree')
     subscription_params = sgqlc.types.Field('ProvisionCustomerSubscriptionInput', graphql_name='subscriptionParams')
 
 
 class ProvisionCustomerSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_information', 'billing_period', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_id')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
     ref_id = sgqlc.types.Field(String, graphql_name='refId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
@@ -2173,19 +2185,20 @@
     __field_names__ = ('billing_model', 'display_name')
     billing_model = sgqlc.types.Field(sgqlc.types.non_null(BillingModel), graphql_name='billingModel')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
 
 
 class ProvisionSubscription(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     checkout_options = sgqlc.types.Field(CheckoutOptions, graphql_name='checkoutOptions')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
@@ -2194,19 +2207,20 @@
     skip_trial = sgqlc.types.Field(Boolean, graphql_name='skipTrial')
     start_date = sgqlc.types.Field(DateTime, graphql_name='startDate')
     subscription_id = sgqlc.types.Field(String, graphql_name='subscriptionId')
 
 
 class ProvisionSubscriptionInput(sgqlc.types.Input):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
+    __field_names__ = ('additional_meta_data', 'addons', 'await_payment_confirmation', 'billing_country_code', 'billing_id', 'billing_information', 'billing_period', 'checkout_options', 'customer_id', 'plan_id', 'price_unit_amount', 'promotion_code', 'ref_id', 'resource_id', 'skip_trial', 'start_date', 'subscription_id')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     addons = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('SubscriptionAddonInput')), graphql_name='addons')
     await_payment_confirmation = sgqlc.types.Field(Boolean, graphql_name='awaitPaymentConfirmation')
     billing_country_code = sgqlc.types.Field(String, graphql_name='billingCountryCode')
+    billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_information = sgqlc.types.Field('SubscriptionBillingInfo', graphql_name='billingInformation')
     billing_period = sgqlc.types.Field(BillingPeriod, graphql_name='billingPeriod')
     checkout_options = sgqlc.types.Field(CheckoutOptions, graphql_name='checkoutOptions')
     customer_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='customerId')
     plan_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='planId')
     price_unit_amount = sgqlc.types.Field(Float, graphql_name='priceUnitAmount')
     promotion_code = sgqlc.types.Field(String, graphql_name='promotionCode')
@@ -3442,15 +3456,15 @@
     __schema__ = schema
     __field_names__ = ('id',)
     id = sgqlc.types.Field(Float, graphql_name='id')
 
 
 class Customer(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'trialed_plans', 'updated_at')
+    __field_names__ = ('additional_meta_data', 'billing_currency', 'billing_id', 'billing_link_url', 'coupon', 'created_at', 'crm_hubspot_company_id', 'crm_hubspot_company_url', 'crm_id', 'customer_id', 'default_payment_expiration_month', 'default_payment_expiration_year', 'default_payment_method_id', 'default_payment_method_last4_digits', 'default_payment_method_type', 'eligible_for_trial', 'email', 'environment', 'environment_id', 'exclude_from_experiment', 'experiment', 'experiment_info', 'has_active_subscription', 'has_payment_method', 'id', 'name', 'promotional_entitlements', 'ref_id', 'subscriptions', 'sync_states', 'trialed_plans', 'updated_at')
     additional_meta_data = sgqlc.types.Field(JSON, graphql_name='additionalMetaData')
     billing_currency = sgqlc.types.Field(Currency, graphql_name='billingCurrency')
     billing_id = sgqlc.types.Field(String, graphql_name='billingId')
     billing_link_url = sgqlc.types.Field(String, graphql_name='billingLinkUrl')
     coupon = sgqlc.types.Field(Coupon, graphql_name='coupon')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     crm_hubspot_company_id = sgqlc.types.Field(String, graphql_name='crmHubspotCompanyId')
@@ -3465,14 +3479,15 @@
     eligible_for_trial = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('EligibleForTrial')), graphql_name='eligibleForTrial')
     email = sgqlc.types.Field(String, graphql_name='email')
     environment = sgqlc.types.Field('Environment', graphql_name='environment')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     exclude_from_experiment = sgqlc.types.Field(Boolean, graphql_name='excludeFromExperiment')
     experiment = sgqlc.types.Field('Experiment', graphql_name='experiment')
     experiment_info = sgqlc.types.Field('experimentInfo', graphql_name='experimentInfo')
+    has_active_subscription = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasActiveSubscription')
     has_payment_method = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hasPaymentMethod')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     name = sgqlc.types.Field(String, graphql_name='name')
     promotional_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null('PromotionalEntitlement'))), graphql_name='promotionalEntitlements', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(PromotionalEntitlementFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(PromotionalEntitlementSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
@@ -3995,21 +4010,22 @@
     entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement))), graphql_name='entitlements')
     environment_id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='environmentId')
     resource_id = sgqlc.types.Field(String, graphql_name='resourceId')
 
 
 class Environment(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('account', 'api_keys', 'created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'is_sandbox', 'provision_status', 'signing_token', 'slug')
+    __field_names__ = ('account', 'api_keys', 'color', 'created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'is_sandbox', 'provision_status', 'signing_token', 'slug')
     account = sgqlc.types.Field(Account, graphql_name='account')
     api_keys = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ApiKey))), graphql_name='apiKeys', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(ApiKeyFilter, graphql_name='filter', default={})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(ApiKeySort)), graphql_name='sorting', default=[])),
 ))
     )
+    color = sgqlc.types.Field(String, graphql_name='color')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='displayName')
     harden_client_access_enabled = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hardenClientAccessEnabled')
     id = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='id')
     is_sandbox = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isSandbox')
     provision_status = sgqlc.types.Field(EnvironmentProvisionStatus, graphql_name='provisionStatus')
@@ -4040,15 +4056,16 @@
     display_name = sgqlc.types.Field(Int, graphql_name='displayName')
     id = sgqlc.types.Field(Int, graphql_name='id')
     slug = sgqlc.types.Field(Int, graphql_name='slug')
 
 
 class EnvironmentDeleteResponse(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'is_sandbox', 'provision_status', 'signing_token', 'slug')
+    __field_names__ = ('color', 'created_at', 'description', 'display_name', 'harden_client_access_enabled', 'id', 'is_sandbox', 'provision_status', 'signing_token', 'slug')
+    color = sgqlc.types.Field(String, graphql_name='color')
     created_at = sgqlc.types.Field(DateTime, graphql_name='createdAt')
     description = sgqlc.types.Field(String, graphql_name='description')
     display_name = sgqlc.types.Field(String, graphql_name='displayName')
     harden_client_access_enabled = sgqlc.types.Field(Boolean, graphql_name='hardenClientAccessEnabled')
     id = sgqlc.types.Field(String, graphql_name='id')
     is_sandbox = sgqlc.types.Field(Boolean, graphql_name='isSandbox')
     provision_status = sgqlc.types.Field(EnvironmentProvisionStatus, graphql_name='provisionStatus')
@@ -6025,15 +6042,15 @@
     __schema__ = schema
     __field_names__ = ('task_id',)
     task_id = sgqlc.types.Field(String, graphql_name='taskId')
 
 
 class Query(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
+    __field_names__ = ('addons', 'cached_entitlements', 'coupon', 'coupons', 'current_environment', 'current_user', 'customer_portal', 'customer_subscriptions', 'customers', 'entitlement', 'entitlements', 'environments', 'experiment', 'experiments', 'features', 'fetch_account', 'get_active_subscriptions', 'get_addon_by_ref_id', 'get_customer_by_ref_id', 'get_experiment_stats', 'get_paywall', 'get_plan_by_ref_id', 'hook', 'hooks', 'import_integration_tasks', 'integrations', 'members', 'mock_paywall', 'package_entitlements', 'paywall', 'plans', 'products', 'promotional_entitlements', 'sdk_configuration', 'send_test_hook', 'stripe_customers', 'stripe_products', 'stripe_subscriptions', 'subscription_entitlements', 'subscription_migration_tasks', 'test_hook_data', 'usage_history', 'usage_measurements', 'widget_configuration')
     addons = sgqlc.types.Field(sgqlc.types.non_null(AddonConnection), graphql_name='addons', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(AddonFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(AddonSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     cached_entitlements = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(Entitlement))), graphql_name='cachedEntitlements', args=sgqlc.types.ArgDict((
@@ -6095,14 +6112,18 @@
     features = sgqlc.types.Field(sgqlc.types.non_null(FeatureConnection), graphql_name='features', args=sgqlc.types.ArgDict((
         ('filter', sgqlc.types.Arg(FeatureFilter, graphql_name='filter', default={})),
         ('paging', sgqlc.types.Arg(CursorPaging, graphql_name='paging', default={'first': 10})),
         ('sorting', sgqlc.types.Arg(sgqlc.types.list_of(sgqlc.types.non_null(FeatureSort)), graphql_name='sorting', default=[{'direction': 'DESC', 'field': 'createdAt'}])),
 ))
     )
     fetch_account = sgqlc.types.Field(Account, graphql_name='fetchAccount')
+    get_active_subscriptions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(CustomerSubscription))), graphql_name='getActiveSubscriptions', args=sgqlc.types.ArgDict((
+        ('input', sgqlc.types.Arg(sgqlc.types.non_null(GetActiveSubscriptionsInput), graphql_name='input', default=None)),
+))
+    )
     get_addon_by_ref_id = sgqlc.types.Field(Addon, graphql_name='getAddonByRefId', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(GetPackageByRefIdInput), graphql_name='input', default=None)),
 ))
     )
     get_customer_by_ref_id = sgqlc.types.Field(Customer, graphql_name='getCustomerByRefId', args=sgqlc.types.ArgDict((
         ('input', sgqlc.types.Arg(sgqlc.types.non_null(GetCustomerByRefIdInput), graphql_name='input', default=None)),
 ))
```

### Comparing `stigg-api-client-0.2.0/setup.py` & `stigg-api-client-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'flake8>=5.0.4,<6.0.0',
  'graphql-core==3.1.6',
  'requests>=2.28.1,<3.0.0',
  'sgqlc>=16.0,<17.0']
 
 setup_kwargs = {
     'name': 'stigg-api-client',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# stigg-api-client\n\nThis library provides a Python wrapper to [Stigg\'s GraphQL API](https://docs.stigg.io/docs/graphql-api) based on \nthe operations that are in use by the [Stigg\'s Node.js SDK](https://docs.stigg.io/docs/nodejs-sdk).\n\nIt leverages the [sgqlc](https://github.com/profusion/sgqlc) library to generate Python classes for GraphQL types, and\nutilizes the `sgqlc.endpoint.requests.RequestsEndpoint` class to send the API requests. The responses are being\nautomatically converted into native Python types.\n\n## Documentation\n\nSee https://docs.stigg.io/docs/python-sdk\n\n## Installation\n\n    pip install stigg-api-client\n\n## Usage\n\nInitialize the client:\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nstigg_client = Stigg.create_client(api_key)\n\n```\n\nProvision a customer\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nclient = Stigg.create_client(api_key)\n\ndata = client.request(Stigg.mutation.provision_customer, {\n    "input": {\n        "refId": "customer-id",\n        "name": "Acme",\n        "email": "hello@acme.com",\n        "couponRefId": "coupon-id",\n        "billingInformation": {\n            "language": "en",\n            "timezone": "America/New_York",\n            "billingAddress": {\n                "country": "US",\n                "city": "New York",\n                "state": "NY",\n                "addressLine1": "123 Main Street",\n                "addressLine2": "Apt. 1",\n                "phoneNumber": "+1 212-499-5321",\n                "postalCode": "10164"\n            },\n            "shippingAddress": {\n                "country": "US",\n                "city": "New York",\n                "state": "NY",\n                "addressLine1": "123 Main Street",\n                "addressLine2": "Apt. 1",\n                "phoneNumber": "+1 212-499-5321",\n                "postalCode": "10164"\n            }\n        },\n        "additionalMetaData": {\n            "key": "value"\n        },\n        "subscriptionParams": {\n            "planId": "plan-revvenu-basic"\n        }\n    }\n})\n\nprint(data.provision_customer.customer.name)\n\n```\n\nGet a customer by ID\n\n```python\n\nimport os\nfrom stigg import Stigg\n\napi_key = os.environ.get("STIGG_SERVER_API_KEY")\n\nclient = Stigg.create_client(api_key)\n\ndata = client.request(Stigg.query.get_customer_by_id, {\n  "input": {"customerId": "customer-id"}\n})\n\ncustomer = data.get_customer_by_ref_id\nprint(customer.name)\n\n```\n',
     'author': 'Stigg',
     'author_email': 'support@stigg.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stigg-api-client-0.2.0/PKG-INFO` & `stigg-api-client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

