# Comparing `tmp/nebari-2023.4.1a4.tar.gz` & `tmp/nebari-2023.4.1a5.tar.gz`

## Comparing `nebari-2023.4.1a4.tar` & `nebari-2023.4.1a5.tar`

### file list

```diff
@@ -1,500 +1,501 @@
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.cirun.yml
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.readthedocs.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/CONTRIBUTING.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/MANIFEST.in
--rw-r--r--   0        0        0    53015 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/RELEASE.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/flake.lock
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/flake.nix
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/noxfile.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/contributor.yaml
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/infracost.yml
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/kubernetes_test.yaml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/markdown.links.config.json
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/release.yaml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.github/workflows/test.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/.gitignore
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/.gitmodules
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/README.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/conf.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/index.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/requirements.txt
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/_templates/announcement.html
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/_templates/layout.html
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/ext/substitute.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/output/.nojekyll
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/argo-workflows.md
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/awss3curl.md
--rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/backup.md
--rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/breaking-upgrade.md
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/clearml.md
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/cost.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/custom-helm-charts.md
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/faq.md
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/gpu.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/index.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/jupyterhub.md
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/keycloak.md
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/monitoring.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/preemptible-spot-instances.md
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/prefect.md
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/system_maintenance.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/traefik.md
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/troubleshooting.md
--rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/admin_guide/upgrade.md
--rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/architecture.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/changelog.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/contribution.md
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/index.md
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/keycloak.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/logo.md
--rw-r--r--   0        0        0    20441 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/minikube.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/release.md
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/dev_guide/testing.md
--rw-r--r--   0        0        0    64293 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/argo-server-landing-page.png
--rw-r--r--   0        0        0   221390 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudfare_update_screenshot.png
--rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudflare_account_resources_scr.png
--rw-r--r--   0        0        0   108690 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudflare_auth_1.png
--rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudflare_permissions_2.1.1.png
--rw-r--r--   0        0        0    75331 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudflare_summary.png
--rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/cloudflare_zone_resources.png
--rw-r--r--   0        0        0   277092 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/dev_postman_for_keycloak.png
--rw-r--r--   0        0        0   154819 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/grafana_manage_dashboards.png
--rw-r--r--   0        0        0    75305 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/grafana_networking_dashboard.png
--rw-r--r--   0        0        0    92141 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/grafana_node_cpu_usage.png
--rw-r--r--   0        0        0    94475 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/high_level_architecture.png
--rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/init_cli_output.png
--rw-r--r--   0        0        0    65086 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/k9s_UI.png
--rw-r--r--   0        0        0   156751 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_add_users.png
--rw-r--r--   0        0        0   161065 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_adduser.png
--rw-r--r--   0        0        0   131930 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_groups.png
--rw-r--r--   0        0        0   132035 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_master_login.png
--rw-r--r--   0        0        0    25405 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_new_group1.png
--rw-r--r--   0        0        0    94386 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_new_group2.png
--rw-r--r--   0        0        0   100928 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_new_group3.png
--rw-r--r--   0        0        0   317402 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_qhub_login.png
--rw-r--r--   0        0        0    97778 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_root_user_account_security.png
--rw-r--r--   0        0        0   157913 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_root_user_manage_account.png
--rw-r--r--   0        0        0   143079 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_root_user_update_password.png
--rw-r--r--   0        0        0   163577 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/keycloak_user_password.png
--rw-r--r--   0        0        0    88640 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/labs_logo_white.png
--rw-r--r--   0        0        0    71430 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_api_token.png
--rw-r--r--   0        0        0    86104 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_api_token_generated.png
--rw-r--r--   0        0        0   185838 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_aws_architecture.png
--rw-r--r--   0        0        0   126188 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_dashboard_notebook.png
--rw-r--r--   0        0        0    63407 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_dashboard_resources.png
--rw-r--r--   0        0        0    56065 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_dashboard_simple.png
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_dask_cluster_options.png
--rw-r--r--   0        0        0    30695 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_dask_cluster_start.png
--rw-r--r--   0        0        0   136024 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_do_architecture.png
--rw-r--r--   0        0        0   136194 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_gcp_architecture.png
--rw-r--r--   0        0        0    75740 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_kernel_selection.png
--rw-r--r--   0        0        0   102949 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_login_screen.png
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_logo.png
--rw-r--r--   0        0        0    44399 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_main_hub_page.png
--rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_new_dashboard.png
--rw-r--r--   0        0        0    61425 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_new_dashboard_filled_in.png
--rw-r--r--   0        0        0    45358 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_notebook.png
--rw-r--r--   0        0        0    69000 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_select_profile.png
--rw-r--r--   0        0        0    57906 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_server_start.png
--rw-r--r--   0        0        0   106710 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/qhub_vscode.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/quansight_logo_white.png
--rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/render_cli_output.png
--rw-r--r--   0        0        0    91557 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/tech_stack_diagram.png
--rw-r--r--   0        0        0    50197 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/training_env.png
--rw-r--r--   0        0        0    47961 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/training_instances.png
--rw-r--r--   0        0        0    57399 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/training_login_1.png
--rw-r--r--   0        0        0    53867 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/training_login_2.png
--rw-r--r--   0        0        0    25284 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/training_server_start.png
--rw-r--r--   0        0        0    38893 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/icons/conda_icon.png
--rw-r--r--   0        0        0    26130 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/icons/dask_icon.png
--rw-r--r--   0        0        0    62475 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/icons/jupyter_hub_icon.png
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/images/icons/nginx_icon.png
--rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/configuration.md
--rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/existing.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/index.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/installation.md
--rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/login.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/management.md
--rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/setup.md
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/installation/usage.md
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/introduction/index.md
--rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/introduction/qhub-101.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/code_server.md
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/dashboard.md
--rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/dask_gateway.md
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/environments.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/experimental.md
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/faq.md
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/getting_started.md
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/idle_culler.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/index.md
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/ssh.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/training.md
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/docs/source/user_guide/troubleshooting.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/__main__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/_version.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/constants.py
--rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cost.py
--rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/deprecate.py
--rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/destroy.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/initialize.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/keycloak.py
--rw-r--r--   0        0        0    12982 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/render.py
--rw-r--r--   0        0        0    17548 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/schema.py
--rw-r--r--   0        0        0    14461 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/upgrade.py
--rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/utils.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cli/__init__.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cli/dev.py
--rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cli/init.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cli/keycloak.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/git.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cicd/common.py
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/stages/__init__.py
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/stages/checks.py
--rw-r--r--   0        0        0    14369 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/stages/input_vars.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/stages/state_imports.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/stages/tf_objects.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/main.tf
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/azure/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/main.tf
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/locals.tf
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/main.tf
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/outputs.tf
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/providers.tf
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/versions.tf
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/existing/main.tf
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/outputs.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/provider.tf
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/main.tf
--rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/metallb.yaml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/outputs.tf
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/variables.tf
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/main.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/versions.tf
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/versions.tf
--rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/outputs.tf
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/versions.tf
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/argo-workflows.tf
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/clearml.tf
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/conda-store.tf
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/forward-auth.tf
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/kbatch.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/locals.tf
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/outputs.tf
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/prefect.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/providers.tf
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
--rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
--rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
--rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
--rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6052 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5139 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    15899 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/jupyterhub.json
--rw-r--r--   0        0        0    52289 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json
--rw-r--r--   0        0        0    30301 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/versions.tf
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0    14303 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/__init__.py
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/conftest.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_cli.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_commons.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_dependencies.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_init.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_links.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_render.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_schema.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/test_upgrade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/notebooks/test-ipython-basic.ipynb
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/scripts/minikube-loadbalancer-ip.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests/vale/styles/vocab.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/constants.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/LICENSE
--rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/README.md
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/pyproject.toml
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 nebari-2023.4.1a4/PKG-INFO
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.cirun.yml
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.readthedocs.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/MANIFEST.in
+-rw-r--r--   0        0        0    53015 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/RELEASE.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/flake.lock
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/flake.nix
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/noxfile.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/contributor.yaml
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/infracost.yml
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/kubernetes_test.yaml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/markdown.links.config.json
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/.gitignore
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/.gitmodules
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/README.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/conf.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/index.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/requirements.txt
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/_templates/announcement.html
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/_templates/layout.html
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/ext/substitute.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/output/.nojekyll
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/argo-workflows.md
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/awss3curl.md
+-rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/backup.md
+-rw-r--r--   0        0        0     7625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/breaking-upgrade.md
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/clearml.md
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/cost.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/custom-helm-charts.md
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/faq.md
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/gpu.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/index.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/jupyterhub.md
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/keycloak.md
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/monitoring.md
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/preemptible-spot-instances.md
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/prefect.md
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/system_maintenance.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/traefik.md
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/troubleshooting.md
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/admin_guide/upgrade.md
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/architecture.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/changelog.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/contribution.md
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/index.md
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/keycloak.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/logo.md
+-rw-r--r--   0        0        0    20441 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/minikube.md
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/release.md
+-rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/dev_guide/testing.md
+-rw-r--r--   0        0        0    64293 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/argo-server-landing-page.png
+-rw-r--r--   0        0        0   221390 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudfare_update_screenshot.png
+-rw-r--r--   0        0        0    17170 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_account_resources_scr.png
+-rw-r--r--   0        0        0   108690 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_auth_1.png
+-rw-r--r--   0        0        0    21474 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_permissions_2.1.1.png
+-rw-r--r--   0        0        0    75331 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_summary.png
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/cloudflare_zone_resources.png
+-rw-r--r--   0        0        0   277092 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/dev_postman_for_keycloak.png
+-rw-r--r--   0        0        0   154819 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_manage_dashboards.png
+-rw-r--r--   0        0        0    75305 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_networking_dashboard.png
+-rw-r--r--   0        0        0    92141 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/grafana_node_cpu_usage.png
+-rw-r--r--   0        0        0    94475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/high_level_architecture.png
+-rw-r--r--   0        0        0    23470 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/init_cli_output.png
+-rw-r--r--   0        0        0    65086 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/k9s_UI.png
+-rw-r--r--   0        0        0   156751 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_add_users.png
+-rw-r--r--   0        0        0   161065 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_adduser.png
+-rw-r--r--   0        0        0   131930 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_groups.png
+-rw-r--r--   0        0        0   132035 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_master_login.png
+-rw-r--r--   0        0        0    25405 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group1.png
+-rw-r--r--   0        0        0    94386 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group2.png
+-rw-r--r--   0        0        0   100928 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_new_group3.png
+-rw-r--r--   0        0        0   317402 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_qhub_login.png
+-rw-r--r--   0        0        0    97778 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_account_security.png
+-rw-r--r--   0        0        0   157913 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_manage_account.png
+-rw-r--r--   0        0        0   143079 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_root_user_update_password.png
+-rw-r--r--   0        0        0   163577 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/keycloak_user_password.png
+-rw-r--r--   0        0        0    88640 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/labs_logo_white.png
+-rw-r--r--   0        0        0    71430 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_api_token.png
+-rw-r--r--   0        0        0    86104 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_api_token_generated.png
+-rw-r--r--   0        0        0   185838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_aws_architecture.png
+-rw-r--r--   0        0        0   126188 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_notebook.png
+-rw-r--r--   0        0        0    63407 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_resources.png
+-rw-r--r--   0        0        0    56065 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dashboard_simple.png
+-rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_options.png
+-rw-r--r--   0        0        0    30695 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_start.png
+-rw-r--r--   0        0        0   136024 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_do_architecture.png
+-rw-r--r--   0        0        0   136194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_gcp_architecture.png
+-rw-r--r--   0        0        0    75740 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_kernel_selection.png
+-rw-r--r--   0        0        0   102949 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_login_screen.png
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_logo.png
+-rw-r--r--   0        0        0    44399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_main_hub_page.png
+-rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard.png
+-rw-r--r--   0        0        0    61425 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard_filled_in.png
+-rw-r--r--   0        0        0    45358 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_notebook.png
+-rw-r--r--   0        0        0    69000 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_select_profile.png
+-rw-r--r--   0        0        0    57906 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_server_start.png
+-rw-r--r--   0        0        0   106710 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/qhub_vscode.png
+-rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/quansight_logo_white.png
+-rw-r--r--   0        0        0    20987 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/render_cli_output.png
+-rw-r--r--   0        0        0    91557 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/tech_stack_diagram.png
+-rw-r--r--   0        0        0    50197 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_env.png
+-rw-r--r--   0        0        0    47961 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_instances.png
+-rw-r--r--   0        0        0    57399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_login_1.png
+-rw-r--r--   0        0        0    53867 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_login_2.png
+-rw-r--r--   0        0        0    25284 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/training_server_start.png
+-rw-r--r--   0        0        0    38893 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/conda_icon.png
+-rw-r--r--   0        0        0    26130 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/dask_icon.png
+-rw-r--r--   0        0        0    62475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/jupyter_hub_icon.png
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/images/icons/nginx_icon.png
+-rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/configuration.md
+-rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/existing.md
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/index.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/installation.md
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/login.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/management.md
+-rw-r--r--   0        0        0    16415 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/setup.md
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/installation/usage.md
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/introduction/index.md
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/introduction/qhub-101.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/code_server.md
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/dashboard.md
+-rw-r--r--   0        0        0     5921 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/dask_gateway.md
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/environments.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/experimental.md
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/faq.md
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/getting_started.md
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/idle_culler.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/index.md
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/ssh.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/training.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/docs/source/user_guide/troubleshooting.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/__main__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/_version.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/constants.py
+-rw-r--r--   0        0        0     8681 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cost.py
+-rw-r--r--   0        0        0    10721 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/deprecate.py
+-rw-r--r--   0        0        0     7139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/destroy.py
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/initialize.py
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/keycloak.py
+-rw-r--r--   0        0        0    12982 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/render.py
+-rw-r--r--   0        0        0    17548 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/schema.py
+-rw-r--r--   0        0        0    14461 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/upgrade.py
+-rw-r--r--   0        0        0    12811 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/utils.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/__init__.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/dev.py
+-rw-r--r--   0        0        0    21893 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/init.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/keycloak.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/git.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/__init__.py
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/checks.py
+-rw-r--r--   0        0        0    14391 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/input_vars.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/state_imports.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/main.tf
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/main.tf
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/locals.tf
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/main.tf
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/outputs.tf
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/main.tf
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/providers.tf
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/versions.tf
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/existing/main.tf
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/outputs.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/provider.tf
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/main.tf
+-rw-r--r--   0        0        0     9383 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/metallb.yaml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/outputs.tf
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/variables.tf
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/main.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/versions.tf
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/initialization/variables.tf
+-rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/versions.tf
+-rw-r--r--   0        0        0     9108 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/outputs.tf
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/versions.tf
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/outputs.tf
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/versions.tf
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/argo-workflows.tf
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/clearml.tf
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/conda-store.tf
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/dask_gateway.tf
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/forward-auth.tf
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/kbatch.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/locals.tf
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/outputs.tf
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/prefect.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/providers.tf
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/versions.tf
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/Chart.yaml
+-rw-r--r--   0        0        0    30585 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml
+-rw-r--r--   0        0        0    52105 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz
+-rw-r--r--   0        0        0    60374 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-agentservices.yaml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-apiserver.yaml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/pvc-fileserver.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secret-agent.yaml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/secrets.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-apiserver.yaml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-fileserver.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/service-webserver.yaml
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    14280 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/values.yaml
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/versions.tf
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    15899 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/jupyterhub.json
+-rw-r--r--   0        0        0    52289 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json
+-rw-r--r--   0        0        0    30301 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/values.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/variables.tf
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/.helmignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/values.yaml
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/providers.tf
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/versions.tf
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0    14303 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/conftest.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_cli.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_commons.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_dependencies.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_init.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_links.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_render.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_schema.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/test_upgrade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/notebooks/test-ipython-basic.ipynb
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/scripts/minikube-loadbalancer-ip.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests/vale/styles/vocab.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/LICENSE
+-rw-r--r--   0        0        0     9701 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/README.md
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/pyproject.toml
+-rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 nebari-2023.4.1a5/PKG-INFO
```

### Comparing `nebari-2023.4.1a4/.cirun.yml` & `nebari-2023.4.1a5/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.pre-commit-config.yaml` & `nebari-2023.4.1a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/CODE_OF_CONDUCT.md` & `nebari-2023.4.1a5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/CONTRIBUTING.md` & `nebari-2023.4.1a5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/RELEASE.md` & `nebari-2023.4.1a5/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/flake.lock` & `nebari-2023.4.1a5/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/flake.nix` & `nebari-2023.4.1a5/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2023.4.1a5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2023.4.1a5/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/contributor.yaml` & `nebari-2023.4.1a5/.github/workflows/contributor.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/infracost.yml` & `nebari-2023.4.1a5/.github/workflows/infracost.yml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/kubernetes_test.yaml` & `nebari-2023.4.1a5/.github/workflows/kubernetes_test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/markdown.links.config.json` & `nebari-2023.4.1a5/.github/workflows/markdown.links.config.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/release-notes-sync.yaml` & `nebari-2023.4.1a5/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/release.yaml` & `nebari-2023.4.1a5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/run-precommit.yaml` & `nebari-2023.4.1a5/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/test-provider.yaml` & `nebari-2023.4.1a5/.github/workflows/test-provider.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.github/workflows/test.yaml` & `nebari-2023.4.1a5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/.gitignore` & `nebari-2023.4.1a5/docs/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/conf.py` & `nebari-2023.4.1a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/index.md` & `nebari-2023.4.1a5/docs/index.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/ext/substitute.py` & `nebari-2023.4.1a5/docs/ext/substitute.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/argo-workflows.md` & `nebari-2023.4.1a5/docs/source/admin_guide/argo-workflows.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/awss3curl.md` & `nebari-2023.4.1a5/docs/source/admin_guide/awss3curl.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/backup.md` & `nebari-2023.4.1a5/docs/source/admin_guide/backup.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/breaking-upgrade.md` & `nebari-2023.4.1a5/docs/source/admin_guide/breaking-upgrade.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/clearml.md` & `nebari-2023.4.1a5/docs/source/admin_guide/clearml.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/cost.md` & `nebari-2023.4.1a5/docs/source/admin_guide/cost.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/custom-helm-charts.md` & `nebari-2023.4.1a5/docs/source/admin_guide/custom-helm-charts.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/faq.md` & `nebari-2023.4.1a5/docs/source/admin_guide/faq.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/gpu.md` & `nebari-2023.4.1a5/docs/source/admin_guide/gpu.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/jupyterhub.md` & `nebari-2023.4.1a5/docs/source/admin_guide/jupyterhub.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/keycloak.md` & `nebari-2023.4.1a5/docs/source/admin_guide/keycloak.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/monitoring.md` & `nebari-2023.4.1a5/docs/source/admin_guide/monitoring.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/preemptible-spot-instances.md` & `nebari-2023.4.1a5/docs/source/admin_guide/preemptible-spot-instances.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/prefect.md` & `nebari-2023.4.1a5/docs/source/admin_guide/prefect.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/system_maintenance.md` & `nebari-2023.4.1a5/docs/source/admin_guide/system_maintenance.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/traefik.md` & `nebari-2023.4.1a5/docs/source/admin_guide/traefik.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/troubleshooting.md` & `nebari-2023.4.1a5/docs/source/admin_guide/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/admin_guide/upgrade.md` & `nebari-2023.4.1a5/docs/source/admin_guide/upgrade.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/architecture.md` & `nebari-2023.4.1a5/docs/source/dev_guide/architecture.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/contribution.md` & `nebari-2023.4.1a5/docs/source/dev_guide/contribution.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/keycloak.md` & `nebari-2023.4.1a5/docs/source/dev_guide/keycloak.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/minikube.md` & `nebari-2023.4.1a5/docs/source/dev_guide/minikube.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/release.md` & `nebari-2023.4.1a5/docs/source/dev_guide/release.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/dev_guide/testing.md` & `nebari-2023.4.1a5/docs/source/dev_guide/testing.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/argo-server-landing-page.png` & `nebari-2023.4.1a5/docs/source/images/argo-server-landing-page.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudfare_update_screenshot.png` & `nebari-2023.4.1a5/docs/source/images/cloudfare_update_screenshot.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudflare_account_resources_scr.png` & `nebari-2023.4.1a5/docs/source/images/cloudflare_account_resources_scr.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudflare_auth_1.png` & `nebari-2023.4.1a5/docs/source/images/cloudflare_auth_1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudflare_permissions_2.1.1.png` & `nebari-2023.4.1a5/docs/source/images/cloudflare_permissions_2.1.1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudflare_summary.png` & `nebari-2023.4.1a5/docs/source/images/cloudflare_summary.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/cloudflare_zone_resources.png` & `nebari-2023.4.1a5/docs/source/images/cloudflare_zone_resources.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/dev_postman_for_keycloak.png` & `nebari-2023.4.1a5/docs/source/images/dev_postman_for_keycloak.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/grafana_manage_dashboards.png` & `nebari-2023.4.1a5/docs/source/images/grafana_manage_dashboards.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/grafana_networking_dashboard.png` & `nebari-2023.4.1a5/docs/source/images/grafana_networking_dashboard.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/grafana_node_cpu_usage.png` & `nebari-2023.4.1a5/docs/source/images/grafana_node_cpu_usage.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/high_level_architecture.png` & `nebari-2023.4.1a5/docs/source/images/high_level_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/init_cli_output.png` & `nebari-2023.4.1a5/docs/source/images/init_cli_output.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/k9s_UI.png` & `nebari-2023.4.1a5/docs/source/images/k9s_UI.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_add_users.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_add_users.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_adduser.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_adduser.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_groups.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_groups.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_master_login.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_master_login.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_new_group1.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_new_group1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_new_group2.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_new_group2.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_new_group3.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_new_group3.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_qhub_login.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_qhub_login.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_root_user_account_security.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_account_security.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_root_user_manage_account.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_manage_account.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_root_user_update_password.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_root_user_update_password.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/keycloak_user_password.png` & `nebari-2023.4.1a5/docs/source/images/keycloak_user_password.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/labs_logo_white.png` & `nebari-2023.4.1a5/docs/source/images/labs_logo_white.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_api_token.png` & `nebari-2023.4.1a5/docs/source/images/qhub_api_token.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_api_token_generated.png` & `nebari-2023.4.1a5/docs/source/images/qhub_api_token_generated.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_aws_architecture.png` & `nebari-2023.4.1a5/docs/source/images/qhub_aws_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_dashboard_notebook.png` & `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_notebook.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_dashboard_resources.png` & `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_resources.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_dashboard_simple.png` & `nebari-2023.4.1a5/docs/source/images/qhub_dashboard_simple.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_dask_cluster_options.png` & `nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_options.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_dask_cluster_start.png` & `nebari-2023.4.1a5/docs/source/images/qhub_dask_cluster_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_do_architecture.png` & `nebari-2023.4.1a5/docs/source/images/qhub_do_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_gcp_architecture.png` & `nebari-2023.4.1a5/docs/source/images/qhub_gcp_architecture.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_kernel_selection.png` & `nebari-2023.4.1a5/docs/source/images/qhub_kernel_selection.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_login_screen.png` & `nebari-2023.4.1a5/docs/source/images/qhub_login_screen.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_logo.png` & `nebari-2023.4.1a5/docs/source/images/qhub_logo.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_main_hub_page.png` & `nebari-2023.4.1a5/docs/source/images/qhub_main_hub_page.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_new_dashboard.png` & `nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_new_dashboard_filled_in.png` & `nebari-2023.4.1a5/docs/source/images/qhub_new_dashboard_filled_in.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_notebook.png` & `nebari-2023.4.1a5/docs/source/images/qhub_notebook.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_select_profile.png` & `nebari-2023.4.1a5/docs/source/images/qhub_select_profile.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_server_start.png` & `nebari-2023.4.1a5/docs/source/images/qhub_server_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/qhub_vscode.png` & `nebari-2023.4.1a5/docs/source/images/qhub_vscode.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/quansight_logo_white.png` & `nebari-2023.4.1a5/docs/source/images/quansight_logo_white.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/render_cli_output.png` & `nebari-2023.4.1a5/docs/source/images/render_cli_output.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/tech_stack_diagram.png` & `nebari-2023.4.1a5/docs/source/images/tech_stack_diagram.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/training_env.png` & `nebari-2023.4.1a5/docs/source/images/training_env.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/training_instances.png` & `nebari-2023.4.1a5/docs/source/images/training_instances.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/training_login_1.png` & `nebari-2023.4.1a5/docs/source/images/training_login_1.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/training_login_2.png` & `nebari-2023.4.1a5/docs/source/images/training_login_2.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/training_server_start.png` & `nebari-2023.4.1a5/docs/source/images/training_server_start.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/icons/conda_icon.png` & `nebari-2023.4.1a5/docs/source/images/icons/conda_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/icons/dask_icon.png` & `nebari-2023.4.1a5/docs/source/images/icons/dask_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/icons/jupyter_hub_icon.png` & `nebari-2023.4.1a5/docs/source/images/icons/jupyter_hub_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/images/icons/nginx_icon.png` & `nebari-2023.4.1a5/docs/source/images/icons/nginx_icon.png`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/configuration.md` & `nebari-2023.4.1a5/docs/source/installation/configuration.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/existing.md` & `nebari-2023.4.1a5/docs/source/installation/existing.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/installation.md` & `nebari-2023.4.1a5/docs/source/installation/installation.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/login.md` & `nebari-2023.4.1a5/docs/source/installation/login.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/management.md` & `nebari-2023.4.1a5/docs/source/installation/management.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/setup.md` & `nebari-2023.4.1a5/docs/source/installation/setup.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/installation/usage.md` & `nebari-2023.4.1a5/docs/source/installation/usage.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/introduction/index.md` & `nebari-2023.4.1a5/docs/source/introduction/index.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/introduction/qhub-101.md` & `nebari-2023.4.1a5/docs/source/introduction/qhub-101.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/code_server.md` & `nebari-2023.4.1a5/docs/source/user_guide/code_server.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/dashboard.md` & `nebari-2023.4.1a5/docs/source/user_guide/dashboard.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/dask_gateway.md` & `nebari-2023.4.1a5/docs/source/user_guide/dask_gateway.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/environments.md` & `nebari-2023.4.1a5/docs/source/user_guide/environments.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/faq.md` & `nebari-2023.4.1a5/docs/source/user_guide/faq.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/getting_started.md` & `nebari-2023.4.1a5/docs/source/user_guide/getting_started.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/idle_culler.md` & `nebari-2023.4.1a5/docs/source/user_guide/idle_culler.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/ssh.md` & `nebari-2023.4.1a5/docs/source/user_guide/ssh.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/training.md` & `nebari-2023.4.1a5/docs/source/user_guide/training.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/docs/source/user_guide/troubleshooting.md` & `nebari-2023.4.1a5/docs/source/user_guide/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/cost.py` & `nebari-2023.4.1a5/nebari/cost.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/deploy.py` & `nebari-2023.4.1a5/nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/destroy.py` & `nebari-2023.4.1a5/nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/initialize.py` & `nebari-2023.4.1a5/nebari/initialize.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/keycloak.py` & `nebari-2023.4.1a5/nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/render.py` & `nebari-2023.4.1a5/nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/schema.py` & `nebari-2023.4.1a5/nebari/schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/upgrade.py` & `nebari-2023.4.1a5/nebari/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/utils.py` & `nebari-2023.4.1a5/nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/version.py` & `nebari-2023.4.1a5/nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/cli/dev.py` & `nebari-2023.4.1a5/nebari/cli/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/cli/init.py` & `nebari-2023.4.1a5/nebari/cli/init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/cli/keycloak.py` & `nebari-2023.4.1a5/nebari/cli/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/cli/main.py` & `nebari-2023.4.1a5/nebari/cli/main.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/git.py` & `nebari-2023.4.1a5/nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/terraform.py` & `nebari-2023.4.1a5/nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cicd/github.py` & `nebari-2023.4.1a5/nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cicd/gitlab.py` & `nebari-2023.4.1a5/nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cicd/linter.py` & `nebari-2023.4.1a5/nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cloud/amazon_web_services.py` & `nebari-2023.4.1a5/nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cloud/azure_cloud.py` & `nebari-2023.4.1a5/nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cloud/digital_ocean.py` & `nebari-2023.4.1a5/nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/cloud/google_cloud.py` & `nebari-2023.4.1a5/nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/dns/cloudflare.py` & `nebari-2023.4.1a5/nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/provider/oauth/auth0.py` & `nebari-2023.4.1a5/nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/stages/checks.py` & `nebari-2023.4.1a5/nebari/stages/checks.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/stages/input_vars.py` & `nebari-2023.4.1a5/nebari/stages/input_vars.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,16 @@
 
     return {
         "realm": realm_id,
         "realm_display_name": config["security"]
         .get("keycloak", {})
         .get("realm_display_name", realm_id),
         "authentication": config["security"]["authentication"],
-        "keycloak_groups": ["admin", "developer", "analyst"] + users_group,
+        "keycloak_groups": ["superadmin", "admin", "developer", "analyst"]
+        + users_group,
         "default_groups": ["analyst"] + users_group,
     }
 
 
 def _split_docker_image_name(image_name):
     name, tag = image_name.split(":")
     return {"name": name, "tag": tag}
```

### Comparing `nebari-2023.4.1a4/nebari/stages/state_imports.py` & `nebari-2023.4.1a5/nebari/stages/state_imports.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/stages/tf_objects.py` & `nebari-2023.4.1a5/nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/azure/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/do/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/01-terraform-state/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/azure/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/metallb.yaml` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/02-infrastructure/local/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/02-infrastructure/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/03-kubernetes-initialize/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/04-kubernetes-ingress/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/05-kubernetes-keycloak/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf` & `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/06-kubernetes-keycloak-configuration/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/argo-workflows.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/clearml.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/clearml.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/conda-store.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/conda-store.tf`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   type        = string
   default     = "quansight/conda-store-server"
 }
 
 variable "conda-store-image-tag" {
   description = "Version of conda-store to use"
   type        = string
-  default     = "v0.4.12"
+  default     = "v0.4.14"
 }
 
 # ====================== RESOURCES =======================
 module "kubernetes-conda-store-server" {
   source = "./modules/kubernetes/services/conda-store"
 
   name      = "nebari"
```

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/dask_gateway.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/dask_gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/jupyterhub.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/kbatch.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/kbatch.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/prefect.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/prefect.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/forwardauth/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/mongodb-10.3.7.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/charts/redis-10.9.0.tgz`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agent.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-agentservices.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-apiserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-elastic.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-fileserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/deployment-webserver.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/clearml/chart/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/server.tf`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,18 @@
 module "conda-store-openid-client" {
   source = "../keycloak-client"
 
   realm_id     = var.realm_id
   client_id    = "conda_store"
   external-url = var.external-url
   role_mapping = {
-    "admin"     = ["conda_store_admin"]
-    "developer" = ["conda_store_developer"]
-    "analyst"   = ["conda_store_developer"]
+    "superadmin" = ["conda_store_superadmin"]
+    "admin"      = ["conda_store_admin"]
+    "developer"  = ["conda_store_developer"]
+    "analyst"    = ["conda_store_developer"]
   }
   callback-url-paths = [
     "https://${var.external-url}/conda-store/oauth_callback"
   ]
 }
```

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 c.S3Storage.access_key = config["minio-username"]
 c.S3Storage.secret_key = config["minio-password"]
 c.S3Storage.region = "us-east-1"  # minio region default
 c.S3Storage.bucket_name = "conda-store"
 
 c.CondaStore.default_namespace = "global"
 c.CondaStore.filesystem_namespace = config["default-namespace"]
+c.CondaStore.conda_allowed_channels = []  # allow all channels
+c.CondaStore.conda_indexed_channels = [
+    "main",
+    "conda-forge",
+    "https://repo.anaconda.com/pkgs/main",
+]
 
 # ==================================
 #        server settings
 # ==================================
 c.CondaStoreServer.log_level = logging.INFO
 c.CondaStoreServer.enable_ui = True
 c.CondaStoreServer.enable_api = True
@@ -89,25 +95,33 @@
             self.user_data_url,
             headers={"Authorization": f"Bearer {oauth_access_token}"},
             verify=self.tls_verify,
         )
         response.raise_for_status()
         user_data = response.json()
 
+        username = user_data["preferred_username"]
+
+        # superadmin gets access to everything
+        if "conda_store_superadmin" in user_data.get("roles", []):
+            return schema.AuthenticationToken(
+                primary_namespace=username,
+                role_bindings={"*/*": {"admin"}},
+            )
+
         role_mappings = {
             "conda_store_admin": "admin",
             "conda_store_developer": "developer",
             "conda_store_viewer": "viewer",
         }
         roles = {
             role_mappings[role]
             for role in user_data.get("roles", [])
             if role in role_mappings
         }
-        username = user_data["preferred_username"]
         default_namespace = config["default-namespace"]
         namespaces = {username, "global", default_namespace}
         role_bindings = {
             f"{username}/*": {"admin"},
             f"{default_namespace}/*": {"viewer"},
             "global/*": roles,
         }
```

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_notebook_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/kbatch/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/jupyterhub.json` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/jupyterhub.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/monitoring/dashboards/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/Chart.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/prefect.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/prefect/chart/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/07-kubernetes-services/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/tf-extensions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf` & `nebari-2023.4.1a5/nebari/template/stages/08-nebari-tf-extensions/modules/nebariextension/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/scripts/aws-force-destroy.py` & `nebari-2023.4.1a5/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/scripts/aws-force-destroy.sh` & `nebari-2023.4.1a5/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/scripts/keycloak-export.py` & `nebari-2023.4.1a5/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/conftest.py` & `nebari-2023.4.1a5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_cli.py` & `nebari-2023.4.1a5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_dependencies.py` & `nebari-2023.4.1a5/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_init.py` & `nebari-2023.4.1a5/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_render.py` & `nebari-2023.4.1a5/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_schema.py` & `nebari-2023.4.1a5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/test_upgrade.py` & `nebari-2023.4.1a5/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2023.4.1a5/tests/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/scripts/minikube-loadbalancer-ip.py` & `nebari-2023.4.1a5/tests/scripts/minikube-loadbalancer-ip.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests/vale/styles/vocab.txt` & `nebari-2023.4.1a5/tests/vale/styles/vocab.txt`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_deployment/test_dask_gateway.py` & `nebari-2023.4.1a5/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2023.4.1a5/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_deployment/utils.py` & `nebari-2023.4.1a5/tests_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2023.4.1a5/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_e2e/package-lock.json` & `nebari-2023.4.1a5/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_e2e/cypress/integration/main.js` & `nebari-2023.4.1a5/tests_e2e/cypress/integration/main.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2023.4.1a5/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_e2e/cypress/plugins/index.js` & `nebari-2023.4.1a5/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/tests_e2e/cypress/support/index.js` & `nebari-2023.4.1a5/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/.gitignore` & `nebari-2023.4.1a5/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/LICENSE` & `nebari-2023.4.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/README.md` & `nebari-2023.4.1a5/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/pyproject.toml` & `nebari-2023.4.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nebari-2023.4.1a4/PKG-INFO` & `nebari-2023.4.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nebari
-Version: 2023.4.1a4
+Version: 2023.4.1a5
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

