# Comparing `tmp/distribute_compute_config-0.14.2.tar.gz` & `tmp/distribute_compute_config-0.14.3.tar.gz`

## Comparing `distribute_compute_config-0.14.2.tar` & `distribute_compute_config-0.14.3.tar`

### file list

```diff
@@ -1,185 +1,189 @@
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/Cargo.toml
--rw-r--r--   0     1001      123     1345 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/.github/workflows/gh-pages.yml
--rw-r--r--   0     1001      123      330 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/.github/workflows/paper-compile.yml
--rw-r--r--   0     1001      123     1512 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/.github/workflows/python.yml
--rw-r--r--   0     1001      123      308 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/.gitignore
--rw-r--r--   0     1001      123    55879 2023-04-06 22:05:12.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/Cargo.lock
--rw-r--r--   0     1001      123    35149 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/LICENSE
--rw-r--r--   0     1001      123      700 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/README.md
--rw-r--r--   0     1001      123        5 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/.gitignore
--rw-r--r--   0     1001      123      264 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/README.md
--rw-r--r--   0     1001      123      110 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/book.toml
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d-utils-exe
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d.x
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/energy_helicity.py
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/proposal_plots.py
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/viscous_dissapation.py
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/vtk-analysis-exe
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-1.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-2.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-3.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_1/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_2/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_3/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-1.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-2.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-3.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_1/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_2/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_3/stdout.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/README.md
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/README.md
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/statistics.csv
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/statistics.csv
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/statistics.csv
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/README.md
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/src/main.f90
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/build.py
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file1.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file2.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file1.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file2.txt
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file3.txt
--rw-r--r--   0     1001      123     9012 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg
--rw-r--r--   0     1001      123   286904 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/architecture.png
--rw-r--r--   0     1001      123   896850 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/architecture.xcf
--rw-r--r--   0     1001      123    14375 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/input_outputs.svg
--rw-r--r--   0     1001      123    15607 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/state_machine.svg
--rw-r--r--   0     1001      123     1012 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/SUMMARY.md
--rw-r--r--   0     1001      123     1030 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/admin_setup.md
--rw-r--r--   0     1001      123     2155 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-input-files.md
--rw-r--r--   0     1001      123     4603 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-introduction.md
--rw-r--r--   0     1001      123     1946 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md
--rw-r--r--   0     1001      123      460 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-packaging-solvers.md
--rw-r--r--   0     1001      123     3440 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-running-locally.md
--rw-r--r--   0     1001      123      642 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-storing-results.md
--rw-r--r--   0     1001      123     6225 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer.md
--rw-r--r--   0     1001      123      682 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/capabilities.md
--rw-r--r--   0     1001      123     8641 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/commands.md
--rw-r--r--   0     1001      123     1405 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/compute_node_setup.md
--rw-r--r--   0     1001      123     7642 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/configuration.md
--rw-r--r--   0     1001      123    93139 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png
--rw-r--r--   0     1001      123    63775 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/figs/input_outputs.png
--rw-r--r--   0     1001      123     1848 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/head_node_setup.md
--rw-r--r--   0     1001      123      613 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/install.md
--rw-r--r--   0     1001      123     3417 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/introduction.md
--rw-r--r--   0     1001      123     1589 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/overview.md
--rw-r--r--   0     1001      123     1628 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-build-scripts.md
--rw-r--r--   0     1001      123     3378 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-execution-scripts.md
--rw-r--r--   0     1001      123      176 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-full-example.md
--rw-r--r--   0     1001      123     3142 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-input-files.md
--rw-r--r--   0     1001      123     1033 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-storing-results.md
--rw-r--r--   0     1001      123     5566 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python.md
--rw-r--r--   0     1001      123      367 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python_api.md
--rw-r--r--   0     1001      123      682 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/build.apptainer
--rw-r--r--   0     1001      123      693 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/build.py
--rw-r--r--   0     1001      123       50 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/dataset_always.csv
--rw-r--r--   0     1001      123       50 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/dataset_sometimes.csv
--rw-r--r--   0     1001      123      481 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/distribute-jobs.yaml
--rw-r--r--   0     1001      123      956 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/run.py
--rw-r--r--   0     1001      123      693 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/build.py
--rw-r--r--   0     1001      123       50 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/dataset_always.csv
--rw-r--r--   0     1001      123       50 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/dataset_sometimes.csv
--rw-r--r--   0     1001      123      543 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/distribute-jobs.yaml
--rw-r--r--   0     1001      123      921 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/run.py
--rw-r--r--   0     1001      123      404 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/install/distribute-compute.service
--rw-r--r--   0     1001      123      510 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/install/distribute-server.service
--rw-r--r--   0     1001      123      470 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/install/setup-root.sh
--rw-r--r--   0     1001      123      699 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/install/setup.sh
--rw-r--r--   0     1001      123      219 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/install/update.sh
--rw-r--r--   0     1001      123      323 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/justfile
--rw-r--r--   0     1001      123    67552 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/paper/node_layout.png
--rw-r--r--   0     1001      123    18914 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/paper/node_layout.svg
--rw-r--r--   0     1001      123     1181 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/paper/paper.bib
--rw-r--r--   0     1001      123     3346 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/paper/paper.md
--rw-r--r--   0     1001      123     4215 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/add.rs
--rw-r--r--   0     1001      123     2991 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/bin/distribute.rs
--rw-r--r--   0     1001      123     9727 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/cli.rs
--rw-r--r--   0     1001      123    13238 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/execute.rs
--rw-r--r--   0     1001      123    14350 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/mod.rs
--rw-r--r--   0     1001      123     7240 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/utils.rs
--rw-r--r--   0     1001      123     7178 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/apptainer.rs
--rw-r--r--   0     1001      123     7020 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/common.rs
--rw-r--r--   0     1001      123     2677 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/hashing.rs
--rw-r--r--   0     1001      123    21664 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/mod.rs
--rw-r--r--   0     1001      123     7562 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/python.rs
--rw-r--r--   0     1001      123     2578 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/requirements.rs
--rw-r--r--   0     1001      123    16061 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/error.rs
--rw-r--r--   0     1001      123      648 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/kill.rs
--rw-r--r--   0     1001      123     4535 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/lib.rs
--rw-r--r--   0     1001      123     1987 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/node_status.rs
--rw-r--r--   0     1001      123     5782 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/pause/mod.rs
--rw-r--r--   0     1001      123     8185 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/pause/unix.rs
--rw-r--r--   0     1001      123     1221 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/prelude.rs
--rw-r--r--   0     1001      123    11745 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/built.rs
--rw-r--r--   0     1001      123    10538 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/compiling.rs
--rw-r--r--   0     1001      123    24554 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/executing.rs
--rw-r--r--   0     1001      123     9073 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/mod.rs
--rw-r--r--   0     1001      123     8218 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/prepare_build.rs
--rw-r--r--   0     1001      123     7335 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/mod.rs
--rw-r--r--   0     1001      123    14228 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/receiver.rs
--rw-r--r--   0     1001      123    12133 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/sender.rs
--rw-r--r--   0     1001      123    12741 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/uninit.rs
--rw-r--r--   0     1001      123     6593 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/pull.rs
--rw-r--r--   0     1001      123     2083 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/run_local.rs
--rw-r--r--   0     1001      123     5431 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/job_pool.rs
--rw-r--r--   0     1001      123     1587 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/matrix.rs
--rw-r--r--   0     1001      123     5640 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/mod.rs
--rw-r--r--   0     1001      123    14011 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/node.rs
--rw-r--r--   0     1001      123     5306 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/pool_data.rs
--rw-r--r--   0     1001      123    34089 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/schedule.rs
--rw-r--r--   0     1001      123    23451 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/user_conn.rs
--rw-r--r--   0     1001      123     4624 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/server_status.rs
--rw-r--r--   0     1001      123    11651 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/slurm.rs
--rw-r--r--   0     1001      123     3413 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/template.rs
--rw-r--r--   0     1001      123    22459 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/src/transport.rs
--rw-r--r--   0     1001      123     1761 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-jobs-apptainer.yaml
--rw-r--r--   0     1001      123     2232 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-jobs-python.yaml
--rw-r--r--   0     1001      123      614 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-nodes.yaml
--rw-r--r--   0     1001      123      165 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/apptainer_local.apt
--rw-r--r--   0     1001      123      447 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/build.sh
--rw-r--r--   0     1001      123      686 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml
--rw-r--r--   0     1001      123       69 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/hello.txt
--rw-r--r--   0     1001      123        3 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/input_1.txt
--rw-r--r--   0     1001      123        3 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/input_2.txt
--rw-r--r--   0     1001      123      715 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/run.py
--rw-r--r--   0     1001      123     3528 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local.rs
--rw-r--r--   0     1001      123      695 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml
--rw-r--r--   0     1001      123      117 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/cancel_job/distribute-nodes.yaml
--rw-r--r--   0     1001      123     4158 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/cancel_job.rs
--rw-r--r--   0     1001      123      117 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_deallocate_jobs/distribute-nodes.yaml
--rw-r--r--   0     1001      123     5304 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_deallocate_jobs.rs
--rw-r--r--   0     1001      123      242 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_pull/distribute-jobs.yaml
--rw-r--r--   0     1001      123       10 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_pull/distribute-nodes.yaml
--rw-r--r--   0     1001      123     6073 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_pull.rs
--rw-r--r--   0     1001      123      309 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/failed_keepalive/distribute-jobs.yaml
--rw-r--r--   0     1001      123      117 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/failed_keepalive/distribute-nodes.yaml
--rw-r--r--   0     1001      123     4939 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/failed_keepalive.rs
--rw-r--r--   0     1001      123      141 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/filter_files/README.md
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/filter_files/nested_folder/another_file.txt
--rw-r--r--   0     1001      123      242 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/pull_large_file/distribute-jobs.yaml
--rw-r--r--   0     1001      123       10 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/pull_large_file/distribute-nodes.yaml
--rw-r--r--   0     1001      123        0 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/python_sleep/build.py
--rw-r--r--   0     1001      123       29 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/python_sleep/sleep30s.py
--rw-r--r--   0     1001      123       30 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/tests/python_sleep/sleep500s.py
--rwxr-xr-x   0     1001      123      523 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/local_dependencies/distribute/update_python_version.sh
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.2/Cargo.toml
--rw-r--r--   0     1001      123      162 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/.readthedocs.yaml
--rw-r--r--   0     1001      123       80 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/MANIFEST.in
--rw-r--r--   0     1001      123      605 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/README.md
--rw-r--r--   0     1001      123     1233 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/distribute_compute_config.pyi
--rw-r--r--   0     1001      123      638 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/make.bat
--rw-r--r--   0     1001      123     1542 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/source/api.rst
--rw-r--r--   0     1001      123     1923 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/source/conf.py
--rw-r--r--   0     1001      123     3545 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/source/example.rst
--rw-r--r--   0     1001      123      836 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/docs/source/index.rst
--rw-r--r--   0     1001      123      176 2023-04-06 22:03:56.000000 distribute_compute_config-0.14.2/pyproject.toml
--rw-r--r--   0     1001      123    14869 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/src/lib.rs
--rw-r--r--   0     1001      123     2307 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/src/validate_bindings.py
--rw-r--r--   0     1001      123     2082 2023-04-06 22:03:52.000000 distribute_compute_config-0.14.2/src/wrap.rs
--rw-r--r--   0     1001      123    17443 2023-04-06 22:05:11.000000 distribute_compute_config-0.14.2/Cargo.lock
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/Cargo.toml
+-rw-r--r--   0     1001      123     1345 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/.github/workflows/gh-pages.yml
+-rw-r--r--   0     1001      123      330 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/.github/workflows/paper-compile.yml
+-rw-r--r--   0     1001      123     1512 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/.github/workflows/python.yml
+-rw-r--r--   0     1001      123      320 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/.gitignore
+-rw-r--r--   0     1001      123    55879 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/Cargo.lock
+-rw-r--r--   0     1001      123    35149 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/LICENSE
+-rw-r--r--   0     1001      123      708 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/README.md
+-rw-r--r--   0     1001      123        5 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/.gitignore
+-rw-r--r--   0     1001      123      264 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/README.md
+-rw-r--r--   0     1001      123      110 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/book.toml
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d-utils-exe
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d.x
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/energy_helicity.py
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/proposal_plots.py
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/viscous_dissapation.py
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/vtk-analysis-exe
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-1.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-2.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-3.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_1/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_2/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_3/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-1.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-2.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-3.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_1/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_2/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_3/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/README.md
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/README.md
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/README.md
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/src/main.f90
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/build.py
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file1.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file2.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file1.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file2.txt
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file3.txt
+-rw-r--r--   0     1001      123     9012 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg
+-rw-r--r--   0     1001      123   286904 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/architecture.png
+-rw-r--r--   0     1001      123   896850 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/architecture.xcf
+-rw-r--r--   0     1001      123    14375 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/input_outputs.svg
+-rw-r--r--   0     1001      123    15607 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/state_machine.svg
+-rw-r--r--   0     1001      123     1012 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/SUMMARY.md
+-rw-r--r--   0     1001      123     1030 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/admin_setup.md
+-rw-r--r--   0     1001      123     2155 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-input-files.md
+-rw-r--r--   0     1001      123     4603 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-introduction.md
+-rw-r--r--   0     1001      123     1946 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md
+-rw-r--r--   0     1001      123      460 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-packaging-solvers.md
+-rw-r--r--   0     1001      123     3440 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-running-locally.md
+-rw-r--r--   0     1001      123      642 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-storing-results.md
+-rw-r--r--   0     1001      123     6225 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer.md
+-rw-r--r--   0     1001      123      682 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/capabilities.md
+-rw-r--r--   0     1001      123     8641 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/commands.md
+-rw-r--r--   0     1001      123     1405 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/compute_node_setup.md
+-rw-r--r--   0     1001      123     7642 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/configuration.md
+-rw-r--r--   0     1001      123    93139 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png
+-rw-r--r--   0     1001      123    63775 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/figs/input_outputs.png
+-rw-r--r--   0     1001      123     1848 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/head_node_setup.md
+-rw-r--r--   0     1001      123      613 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/install.md
+-rw-r--r--   0     1001      123     3417 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/introduction.md
+-rw-r--r--   0     1001      123     1589 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/overview.md
+-rw-r--r--   0     1001      123     1628 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-build-scripts.md
+-rw-r--r--   0     1001      123     3378 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-execution-scripts.md
+-rw-r--r--   0     1001      123      176 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-full-example.md
+-rw-r--r--   0     1001      123     3142 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-input-files.md
+-rw-r--r--   0     1001      123     1033 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-storing-results.md
+-rw-r--r--   0     1001      123     5566 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python.md
+-rw-r--r--   0     1001      123      367 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python_api.md
+-rw-r--r--   0     1001      123      682 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/build.apptainer
+-rw-r--r--   0     1001      123      693 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/build.py
+-rw-r--r--   0     1001      123       50 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/dataset_always.csv
+-rw-r--r--   0     1001      123       50 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/dataset_sometimes.csv
+-rw-r--r--   0     1001      123      481 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      956 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/run.py
+-rw-r--r--   0     1001      123      693 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/build.py
+-rw-r--r--   0     1001      123       50 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/dataset_always.csv
+-rw-r--r--   0     1001      123       50 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/dataset_sometimes.csv
+-rw-r--r--   0     1001      123      543 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      921 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/run.py
+-rw-r--r--   0     1001      123      404 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/install/distribute-compute.service
+-rw-r--r--   0     1001      123      510 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/install/distribute-server.service
+-rw-r--r--   0     1001      123      470 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/install/setup-root.sh
+-rw-r--r--   0     1001      123      699 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/install/setup.sh
+-rw-r--r--   0     1001      123      219 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/install/update.sh
+-rw-r--r--   0     1001      123      323 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/justfile
+-rw-r--r--   0     1001      123    63775 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/paper/input_outputs.png
+-rw-r--r--   0     1001      123    67552 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/paper/node_layout.png
+-rw-r--r--   0     1001      123    18914 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/paper/node_layout.svg
+-rw-r--r--   0     1001      123     1420 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/paper/paper.bib
+-rw-r--r--   0     1001      123     6333 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/paper/paper.md
+-rw-r--r--   0     1001      123     4357 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/add.rs
+-rw-r--r--   0     1001      123     2991 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/bin/distribute.rs
+-rw-r--r--   0     1001      123     9727 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/cli.rs
+-rw-r--r--   0     1001      123    13238 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/execute.rs
+-rw-r--r--   0     1001      123    14350 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/mod.rs
+-rw-r--r--   0     1001      123     7240 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/utils.rs
+-rw-r--r--   0     1001      123     8290 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/apptainer.rs
+-rw-r--r--   0     1001      123     7181 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/common.rs
+-rw-r--r--   0     1001      123     2677 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/hashing.rs
+-rw-r--r--   0     1001      123    21876 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/mod.rs
+-rw-r--r--   0     1001      123     7562 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/python.rs
+-rw-r--r--   0     1001      123     2650 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/requirements.rs
+-rw-r--r--   0     1001      123    16061 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/error.rs
+-rw-r--r--   0     1001      123      648 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/kill.rs
+-rw-r--r--   0     1001      123     4990 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/lib.rs
+-rw-r--r--   0     1001      123     1993 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/node_status.rs
+-rw-r--r--   0     1001      123     5782 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/pause/mod.rs
+-rw-r--r--   0     1001      123     8185 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/pause/unix.rs
+-rw-r--r--   0     1001      123     1221 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/prelude.rs
+-rw-r--r--   0     1001      123    11560 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/built.rs
+-rw-r--r--   0     1001      123    10356 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/compiling.rs
+-rw-r--r--   0     1001      123    24595 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/executing.rs
+-rw-r--r--   0     1001      123     9723 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/mod.rs
+-rw-r--r--   0     1001      123     8065 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/prepare_build.rs
+-rw-r--r--   0     1001      123     7655 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/mod.rs
+-rw-r--r--   0     1001      123    13968 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/receiver.rs
+-rw-r--r--   0     1001      123    13724 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/sender.rs
+-rw-r--r--   0     1001      123    12649 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/uninit.rs
+-rw-r--r--   0     1001      123     6599 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/pull.rs
+-rw-r--r--   0     1001      123     2089 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/run_local.rs
+-rw-r--r--   0     1001      123     5820 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/job_pool.rs
+-rw-r--r--   0     1001      123     1587 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/matrix.rs
+-rw-r--r--   0     1001      123     5646 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/mod.rs
+-rw-r--r--   0     1001      123    14370 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/node.rs
+-rw-r--r--   0     1001      123     7584 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/pool_data.rs
+-rw-r--r--   0     1001      123    34089 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/schedule.rs
+-rw-r--r--   0     1001      123    23451 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/user_conn.rs
+-rw-r--r--   0     1001      123     4624 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/server_status.rs
+-rw-r--r--   0     1001      123    11657 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/slurm.rs
+-rw-r--r--   0     1001      123     3413 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/template.rs
+-rw-r--r--   0     1001      123    21028 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/src/transport.rs
+-rw-r--r--   0     1001      123     1761 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-jobs-apptainer.yaml
+-rw-r--r--   0     1001      123     2232 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-jobs-python.yaml
+-rw-r--r--   0     1001      123      614 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-nodes.yaml
+-rw-r--r--   0     1001      123      165 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/apptainer_local.apt
+-rw-r--r--   0     1001      123      447 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/build.sh
+-rw-r--r--   0     1001      123      686 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       69 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/hello.txt
+-rw-r--r--   0     1001      123        3 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/input_1.txt
+-rw-r--r--   0     1001      123        3 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/input_2.txt
+-rw-r--r--   0     1001      123      715 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/run.py
+-rw-r--r--   0     1001      123     3528 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local.rs
+-rw-r--r--   0     1001      123      695 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/cancel_job/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     4158 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/cancel_job.rs
+-rw-r--r--   0     1001      123      117 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_deallocate_jobs/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     5304 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_deallocate_jobs.rs
+-rw-r--r--   0     1001      123      242 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_pull/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       10 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_pull/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     6073 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_pull.rs
+-rw-r--r--   0     1001      123      309 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/failed_keepalive/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/failed_keepalive/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     4939 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/failed_keepalive.rs
+-rw-r--r--   0     1001      123      141 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/filter_files/README.md
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/filter_files/nested_folder/another_file.txt
+-rw-r--r--   0     1001      123      396 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     7320 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/many_jobsets_single_sif.rs
+-rw-r--r--   0     1001      123      242 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/pull_large_file/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       10 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/pull_large_file/distribute-nodes.yaml
+-rw-r--r--   0     1001      123        0 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/python_sleep/build.py
+-rw-r--r--   0     1001      123       29 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/python_sleep/sleep30s.py
+-rw-r--r--   0     1001      123       30 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/tests/python_sleep/sleep500s.py
+-rwxr-xr-x   0     1001      123      523 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/local_dependencies/distribute/update_python_version.sh
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.3/Cargo.toml
+-rw-r--r--   0     1001      123      162 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/.readthedocs.yaml
+-rw-r--r--   0     1001      123       80 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/MANIFEST.in
+-rw-r--r--   0     1001      123      605 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/README.md
+-rw-r--r--   0     1001      123     1233 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/distribute_compute_config.pyi
+-rw-r--r--   0     1001      123      638 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/make.bat
+-rw-r--r--   0     1001      123     1542 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/source/api.rst
+-rw-r--r--   0     1001      123     1923 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/source/conf.py
+-rw-r--r--   0     1001      123     3545 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/source/example.rst
+-rw-r--r--   0     1001      123      836 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/docs/source/index.rst
+-rw-r--r--   0     1001      123      176 2023-04-11 00:39:03.000000 distribute_compute_config-0.14.3/pyproject.toml
+-rw-r--r--   0     1001      123    14869 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/src/lib.rs
+-rw-r--r--   0     1001      123     2307 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/src/validate_bindings.py
+-rw-r--r--   0     1001      123     2082 2023-04-11 00:38:57.000000 distribute_compute_config-0.14.3/src/wrap.rs
+-rw-r--r--   0     1001      123    17443 2023-04-11 00:40:11.000000 distribute_compute_config-0.14.3/Cargo.lock
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.3/PKG-INFO
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/Cargo.toml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "distribute"
-version = "0.14.2"
+version = "0.14.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/.github/workflows/gh-pages.yml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/.github/workflows/python.yml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/Cargo.lock` & `distribute_compute_config-0.14.3/local_dependencies/distribute/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "distribute"
-version = "0.14.2"
+version = "0.14.3"
 dependencies = [
  "base16",
  "bincode",
  "chrono",
  "clap",
  "derive_more",
  "futures",
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/LICENSE` & `distribute_compute_config-0.14.3/local_dependencies/distribute/LICENSE`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/README.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 easy to use distributed computing
 
 ## Installing
 
 You will need a recent version of `cargo` and the rust compiler `rustc`. Install instructions are [here](https://www.rust-lang.org/tools/install)
 
-```
+```bash
 cargo install --git "https://github.com/fluid-Dynamics-Group/distribute" --force
 ```
 
 ## Documentation:
 
 User documentation (which you are most likely interested in) is hosted on github: https://fluid-dynamics-group.github.io/distribute
 
 Developer documentation is built with
 
-```
+```bash
 cargo doc --no-deps --open
 ```
 
 ## Features
 
 If you are using `distribute` as a library, one of the following features *must* be selected for the crate to compile
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/architecture.png` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/architecture.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/architecture.xcf` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/architecture.xcf`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/input_outputs.svg` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/input_outputs.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/figs/state_machine.svg` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/figs/state_machine.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/SUMMARY.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/admin_setup.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/admin_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-input-files.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-input-files.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-introduction.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-introduction.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-running-locally.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-running-locally.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer-storing-results.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer-storing-results.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/apptainer.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/apptainer.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/capabilities.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/capabilities.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/commands.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/commands.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/compute_node_setup.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/compute_node_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/configuration.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/configuration.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/figs/input_outputs.png` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/figs/input_outputs.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/head_node_setup.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/head_node_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/install.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/introduction.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/introduction.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/overview.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/overview.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-build-scripts.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-build-scripts.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-execution-scripts.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-execution-scripts.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-input-files.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-input-files.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python-storing-results.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python-storing-results.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/docs/src/python.md` & `distribute_compute_config-0.14.3/local_dependencies/distribute/docs/src/python.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/build.apptainer` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/build.apptainer`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/build.py` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/build.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/apptainer/run.py` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/apptainer/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/build.py` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/build.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/distribute-jobs.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/examples/python/run.py` & `distribute_compute_config-0.14.3/local_dependencies/distribute/examples/python/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/install/setup.sh` & `distribute_compute_config-0.14.3/local_dependencies/distribute/install/setup.sh`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/paper/node_layout.png` & `distribute_compute_config-0.14.3/local_dependencies/distribute/paper/node_layout.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/paper/node_layout.svg` & `distribute_compute_config-0.14.3/local_dependencies/distribute/paper/node_layout.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/paper/paper.bib` & `distribute_compute_config-0.14.3/local_dependencies/distribute/paper/paper.bib`

 * *Files 12% similar despite different names*

```diff
@@ -23,7 +23,16 @@
   booktitle={2016 IEEE High Performance Extreme Computing Conference (HPEC)},
   pages={1--6},
   year={2016},
   organization={IEEE},
   url={https://doi.org/10.1109/hpec.2016.7761604},
   doi={10.1109/hpec.2016.7761604}
 }
+
+@misc{apptainer,
+  author = {Apptainer Collaboration},
+  title = {Apptainer: Application containers for Linux },
+  year = {2022},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  url = {https://github.com/apptainer/apptainer}
+}
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/add.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/add.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use crate::prelude::*;
 
 /// add a job batch to the head node
 pub async fn add(args: cli::Add) -> Result<(), Error> {
     //
     // load the config files
     //
-    let config = config::load_config::<config::Jobs<config::common::File>>(&args.jobs)?;
+    let config = config::load_config::<config::Jobs<config::common::File>>(&args.jobs, true)?;
 
     if config.len_jobs() == 0 {
         return Err(Error::Add(error::AddError::NoJobsToAdd));
     }
 
     // ensure that there are no duplicate job names
     check_has_duplicates(&config.job_names()).map_err(error::AddError::from)?;
@@ -92,14 +92,18 @@
     //
     // send all the files with send_files state machine
     //
     let conn = conn.update_state();
 
     let extra = protocol::send_files::FlatFileList {
         files: hashed_files_to_send,
+        node_meta: server::pool_data::NodeMetadata {
+            node_name: "SERVER".into(),
+            node_address: addr,
+        },
     };
     let state = protocol::send_files::SenderState { conn, extra };
     let machine = protocol::Machine::from_state(state);
 
     let mut conn: transport::Connection<transport::UserMessageToServer> =
         match machine.send_files().await {
             Ok(next) => next.into_inner().update_state(),
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/bin/distribute.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/bin/distribute.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/cli.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/cli.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/execute.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/execute.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/client/utils.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/client/utils.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/apptainer.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/python.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use super::NormalizePaths;
-use derive_more::Constructor;
 
+// event though these are included in the prelude, the prelude only exists for the cli
+// feature
+use derive_more::Constructor;
 use serde::{Deserialize, Serialize};
 use std::path::PathBuf;
 
 use super::common;
 
 #[cfg(feature = "cli")]
 use super::hashing;
@@ -12,28 +14,28 @@
 #[cfg(feature = "cli")]
 use crate::client::execute::FileMetadata;
 
 use getset::Getters;
 
 #[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
 #[serde(deny_unknown_fields)]
-/// initialization and job specification for apptainer job batches
+/// initialization and job specification for python job batches
 pub struct Description<FILE> {
     #[getset(get = "pub(crate)")]
-    /// initialization information on apptainer job
+    /// initialization information on how to compile the job batch
     pub initialize: Initialize<FILE>,
     #[getset(get = "pub(crate)")]
-    /// list of jobs to execute in the job batch
+    /// list of jobs to execute with the given initialization
     pub jobs: Vec<Job<FILE>>,
 }
 
 #[cfg(feature = "cli")]
 impl Description<common::File> {
     pub(super) fn verify_config(&self) -> Result<(), super::MissingFilename> {
-        self.initialize.sif.exists_or_err()?;
+        self.initialize.python_build_file_path().exists_or_err()?;
 
         self.initialize
             .required_files
             .iter()
             .try_for_each(|f| f.exists_or_err())?;
 
         self.jobs.iter().try_for_each(|job| {
@@ -51,20 +53,21 @@
 
     pub(super) fn hashed(
         &self,
         meta: &super::Meta,
     ) -> Result<Description<common::HashedFile>, super::MissingFilename> {
         let initialize = self.initialize.hashed(meta)?;
 
-        let jobs = self
-            .jobs
-            .iter()
-            .enumerate()
-            .map(|(job_idx, job)| job.hashed(job_idx, meta))
-            .collect::<Result<Vec<_>, super::MissingFilename>>()?;
+        let mut jobs = Vec::new();
+
+        for (job_idx, job) in self.jobs.iter().enumerate() {
+            let hashed_job = job.hashed(job_idx, meta)?;
+
+            jobs.push(hashed_job);
+        }
 
         let desc = Description { initialize, jobs };
 
         Ok(desc)
     }
 }
 
@@ -85,61 +88,59 @@
 
 impl<FILE> NormalizePaths for Description<FILE>
 where
     FILE: NormalizePaths,
 {
     fn normalize_paths(&mut self, base: PathBuf) {
         // for initialize
-        self.initialize.sif.normalize_paths(base.clone());
+        self.initialize
+            .python_build_file_path
+            .normalize_paths(base.clone());
 
         for file in self.initialize.required_files.iter_mut() {
             file.normalize_paths(base.clone());
         }
 
         // for jobs
         for job in self.jobs.iter_mut() {
+            job.python_job_file.normalize_paths(base.clone());
+
             for file in job.required_files.iter_mut() {
                 file.normalize_paths(base.clone())
             }
         }
     }
 }
 
 #[derive(Debug, Clone, Deserialize, Serialize, Constructor, getset::Getters)]
 #[serde(deny_unknown_fields)]
 /// initialization information for python jobs
 pub struct Initialize<FILE> {
+    #[serde(rename = "build_file")]
     #[getset(get = "pub(crate)")]
-    /// path to .sif file generated from apptainer
-    pub sif: FILE,
-    #[serde(default = "Default::default")]
-    #[getset(get = "pub(crate)")]
-    /// list of required files used in apptainer initialization. Generally, for apptainer jobs,
-    /// these are simply files that will always be present
-    pub required_files: Vec<FILE>,
-    /// paths in the folder that need to have mount points to
-    /// the host file system
+    /// path to build file for python job batch
+    pub python_build_file_path: FILE,
     #[serde(default = "Default::default")]
     #[getset(get = "pub(crate)")]
-    pub required_mounts: Vec<PathBuf>,
+    /// list of required files used in compilation script
+    pub(super) required_files: Vec<FILE>,
 }
 
 #[cfg(feature = "cli")]
 impl Initialize<common::File> {
-    fn hashed(
+    pub(crate) fn hashed(
         &self,
         meta: &super::Meta,
     ) -> Result<Initialize<common::HashedFile>, super::MissingFilename> {
         let init_hash = hashing::filename_hash(self, meta);
 
-        // hash the sif
-        let hashed_path = format!("setup_sif_{init_hash}.dist").into();
-        let unhashed_path = self.sif.path().into();
-        let filename = self.sif.filename()?;
-        let sif = common::HashedFile::new(hashed_path, unhashed_path, filename);
+        let hashed_path = format!("setup_python_{init_hash}.dist").into();
+        let unhashed_path = self.python_build_file_path.path().into();
+        let filename = self.python_build_file_path.filename()?;
+        let python_build_file_path = common::HashedFile::new(hashed_path, unhashed_path, filename);
 
         // hashed required files
         let required_files = self
             .required_files
             .iter()
             .enumerate()
             .map(|(idx, init_file)| {
@@ -151,61 +152,59 @@
                     unhashed_path,
                     filename,
                 ))
             })
             .collect::<Result<Vec<_>, super::MissingFilename>>()?;
 
         let init = Initialize {
-            sif,
+            python_build_file_path,
             required_files,
-            required_mounts: self.required_mounts.clone(),
         };
 
         Ok(init)
     }
 }
 
 #[cfg(feature = "cli")]
 impl Initialize<common::HashedFile> {
-    pub(super) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
-        files.push(self.sif.as_sendable(is_user));
+    pub(crate) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
+        files.push(self.python_build_file_path.as_sendable(is_user));
 
         self.required_files
             .iter()
             .for_each(|hashed_file| files.push(hashed_file.as_sendable(is_user)));
     }
 }
 
-#[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
+#[derive(Debug, Clone, Deserialize, Serialize, Constructor, getset::Getters)]
 #[serde(deny_unknown_fields)]
-/// specification for an apptainer job
+/// specification for a python job
 pub struct Job<FILE> {
     #[getset(get = "pub(crate)")]
-    name: String,
+    pub(super) name: String,
+    #[serde(rename = "file")]
+    #[getset(get = "pub(crate)")]
+    pub(super) python_job_file: FILE,
     #[serde(default = "Default::default")]
     #[getset(get = "pub(crate)")]
-    /// files required for the execution of this job
-    pub required_files: Vec<FILE>,
+    pub(super) required_files: Vec<FILE>,
     /// slurm configuration. This level of information will override the defeaults at the outer
     /// most level of the configuration
-    #[getset(get = "pub(crate)")]
     slurm: Option<super::Slurm>,
 }
 
 #[cfg(feature = "cli")]
 impl Job<common::File> {
     pub(crate) fn hashed(
         &self,
         job_idx: usize,
         meta: &super::Meta,
     ) -> Result<Job<common::HashedFile>, super::MissingFilename> {
-        //
-        // for each job ...
-        //
         let hash = hashing::filename_hash(self, meta);
+
         let required_files = self
             .required_files
             .iter()
             .enumerate()
             .map(|(file_idx, file)| {
                 //
                 // for each file in this job ...
@@ -218,25 +217,34 @@
                     hashed_path,
                     unhashed_path,
                     filename,
                 ))
             })
             .collect::<Result<Vec<_>, super::MissingFilename>>()?;
 
+        let hashed_path = format!("{hash}_python_run.dist").into();
+        let unhashed_path = self.python_job_file.path().into();
+        let filename = self.python_job_file.filename()?;
+        let python_job_file = common::HashedFile::new(hashed_path, unhashed_path, filename);
+
         // assemble the new files into a new job
         let job = Job {
             name: self.name().to_string(),
+            python_job_file,
             required_files,
             slurm: self.slurm.clone(),
         };
 
         Ok(job)
     }
 }
+
 #[cfg(feature = "cli")]
 impl Job<common::HashedFile> {
     pub(crate) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
+        files.push(self.python_job_file.as_sendable(is_user));
+
         self.required_files
             .iter()
             .for_each(|hashed_file| files.push(hashed_file.as_sendable(is_user)));
     }
 }
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/common.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/common.rs`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 /// present in configuration files.
 pub struct HashedFile {
     // on the server, this is the absolute path to the file on disk
     //
     // on the user's computer, this is a relative path that only contains the hash of the file
     // so that the file will be dumped precisely where we intend it to be dumped on the server
     // through send_files
+    #[getset(get = "pub(crate)")]
     hashed_path: PathBuf,
     // on the user's computer, this is the absolute path to the file
     //
     // on the server, this is not really used
     unhashed_path_user: PathBuf,
     // the path to the file locally
     #[getset(get = "pub(crate)")]
@@ -196,14 +197,15 @@
             self.hashed_path.clone(),
             // location we intend to send this to
             PathBuf::from(self.original_filename.clone()),
         )
     }
 
     pub(super) fn delete_at_hashed_path(&self) -> Result<(), std::io::Error> {
+        debug!(hashed_path = %self.hashed_path.display(), original_filename = self.original_filename, "deleting hashed file");
         std::fs::remove_file(&self.hashed_path)?;
 
         Ok(())
     }
 }
 
 impl NormalizePaths for HashedFile {
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/hashing.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/hashing.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 use serde::de::DeserializeOwned;
 use serde::{Deserialize, Serialize};
 use std::io::Write;
 use std::path::Path;
 use std::path::PathBuf;
 
 use getset::Getters;
+use getset::Setters;
 
 macro_rules! const_port {
     ($NUMERIC:ident, $STR:ident, $value:expr, $docstring:expr) => {
         #[doc=$docstring]
         pub const $NUMERIC: u16 = $value;
         #[doc=$docstring]
         pub const $STR: &'static str = stringify!($value);
@@ -243,18 +244,20 @@
 
 #[derive(
     Debug, Clone, Deserialize, Serialize, Constructor, getset::Getters, getset::MutGetters,
 )]
 #[serde(deny_unknown_fields)]
 /// apptainer configuration file
 pub struct ApptainerConfig<FILE> {
-    #[getset(get = "pub(crate)")]
+    /// Getters for configuration metadata
+    #[getset(get = "pub(crate)", get_mut = "pub")]
     meta: Meta,
     #[serde(rename = "apptainer")]
-    #[getset(get = "pub(crate)", get_mut = "pub(crate)")]
+    #[getset(get = "pub(crate)", get_mut = "pub")]
+    /// description of the initialization and jobs for this config
     description: apptainer::Description<FILE>,
     #[getset(get = "pub(crate)")]
     slurm: Option<Slurm>,
 }
 
 #[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
 #[serde(deny_unknown_fields)]
@@ -362,19 +365,19 @@
     pub(crate) fn placeholder_python(file: common::File) -> Self {
         let file = file.hashed().unwrap();
         let job = python::Job::new("python".into(), file, vec![], None);
         Self::from(job)
     }
 }
 
-#[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
+#[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters, Setters)]
 #[serde(deny_unknown_fields)]
 /// A container for the `meta:` section of a distribute-jobs.yaml file
 pub struct Meta {
-    #[getset(get = "pub(crate)")]
+    #[getset(get = "pub(crate)", set = "pub")]
     /// the batch name for the job set
     pub batch_name: String,
     #[getset(get = "pub(crate)")]
     /// the namespace for the job set
     pub namespace: String,
     /// the matrix user to message on completion
     pub matrix: Option<matrix_notify::OwnedUserId>,
@@ -537,14 +540,15 @@
         // we dont actually need to normalize things for nodes configuration
     }
 }
 
 /// read in a config file from disk
 pub fn load_config<T: DeserializeOwned + NormalizePaths>(
     path: &Path,
+    normalize: bool
 ) -> Result<T, ConfigurationError> {
     let file = std::fs::File::open(path).map_err(|e| {
         ConfigurationError::new(path.display().to_string(), ConfigErrorReason::from(e))
     })?;
 
     let config: Result<T, _> = serde_yaml::from_reader(file);
 
@@ -571,15 +575,17 @@
                 path.display().to_string(),
                 ConfigErrorReason::from(deser_error),
             ));
         }
         Ok(config) => config,
     };
 
-    config.normalize_paths(path.parent().unwrap().to_owned());
+    if normalize {
+        config.normalize_paths(path.parent().unwrap().to_owned());
+    }
 
     Ok(config)
 }
 
 #[derive(Deserialize, Serialize, Clone, Debug, getset::Getters, Constructor)]
 #[cfg_attr(feature = "python", pyo3::pyclass)]
 /// fields that can be serialized to slurm parameters
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/python.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/apptainer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 use super::NormalizePaths;
-
-// event though these are included in the prelude, the prelude only exists for the cli
-// feature
 use derive_more::Constructor;
+
 use serde::{Deserialize, Serialize};
 use std::path::PathBuf;
 
 use super::common;
 
 #[cfg(feature = "cli")]
 use super::hashing;
@@ -14,28 +12,28 @@
 #[cfg(feature = "cli")]
 use crate::client::execute::FileMetadata;
 
 use getset::Getters;
 
 #[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
 #[serde(deny_unknown_fields)]
-/// initialization and job specification for python job batches
+/// initialization and job specification for apptainer job batches
 pub struct Description<FILE> {
-    #[getset(get = "pub(crate)")]
-    /// initialization information on how to compile the job batch
+    #[getset(get = "pub(crate)", get_mut = "pub")]
+    /// initialization information on apptainer job
     pub initialize: Initialize<FILE>,
     #[getset(get = "pub(crate)")]
-    /// list of jobs to execute with the given initialization
+    /// list of jobs to execute in the job batch
     pub jobs: Vec<Job<FILE>>,
 }
 
 #[cfg(feature = "cli")]
 impl Description<common::File> {
     pub(super) fn verify_config(&self) -> Result<(), super::MissingFilename> {
-        self.initialize.python_build_file_path().exists_or_err()?;
+        self.initialize.sif.exists_or_err()?;
 
         self.initialize
             .required_files
             .iter()
             .try_for_each(|f| f.exists_or_err())?;
 
         self.jobs.iter().try_for_each(|job| {
@@ -53,21 +51,20 @@
 
     pub(super) fn hashed(
         &self,
         meta: &super::Meta,
     ) -> Result<Description<common::HashedFile>, super::MissingFilename> {
         let initialize = self.initialize.hashed(meta)?;
 
-        let mut jobs = Vec::new();
-
-        for (job_idx, job) in self.jobs.iter().enumerate() {
-            let hashed_job = job.hashed(job_idx, meta)?;
-
-            jobs.push(hashed_job);
-        }
+        let jobs = self
+            .jobs
+            .iter()
+            .enumerate()
+            .map(|(job_idx, job)| job.hashed(job_idx, meta))
+            .collect::<Result<Vec<_>, super::MissingFilename>>()?;
 
         let desc = Description { initialize, jobs };
 
         Ok(desc)
     }
 }
 
@@ -88,59 +85,61 @@
 
 impl<FILE> NormalizePaths for Description<FILE>
 where
     FILE: NormalizePaths,
 {
     fn normalize_paths(&mut self, base: PathBuf) {
         // for initialize
-        self.initialize
-            .python_build_file_path
-            .normalize_paths(base.clone());
+        self.initialize.sif.normalize_paths(base.clone());
 
         for file in self.initialize.required_files.iter_mut() {
             file.normalize_paths(base.clone());
         }
 
         // for jobs
         for job in self.jobs.iter_mut() {
-            job.python_job_file.normalize_paths(base.clone());
-
             for file in job.required_files.iter_mut() {
                 file.normalize_paths(base.clone())
             }
         }
     }
 }
 
 #[derive(Debug, Clone, Deserialize, Serialize, Constructor, getset::Getters)]
 #[serde(deny_unknown_fields)]
 /// initialization information for python jobs
 pub struct Initialize<FILE> {
-    #[serde(rename = "build_file")]
     #[getset(get = "pub(crate)")]
-    /// path to build file for python job batch
-    pub python_build_file_path: FILE,
+    /// path to .sif file generated from apptainer
+    pub sif: FILE,
     #[serde(default = "Default::default")]
     #[getset(get = "pub(crate)")]
-    /// list of required files used in compilation script
-    pub(super) required_files: Vec<FILE>,
+    /// list of required files used in apptainer initialization. Generally, for apptainer jobs,
+    /// these are simply files that will always be present
+    pub required_files: Vec<FILE>,
+    /// paths in the folder that need to have mount points to
+    /// the host file system
+    #[serde(default = "Default::default")]
+    #[getset(get = "pub(crate)")]
+    pub required_mounts: Vec<PathBuf>,
 }
 
 #[cfg(feature = "cli")]
 impl Initialize<common::File> {
-    pub(crate) fn hashed(
+    fn hashed(
         &self,
         meta: &super::Meta,
     ) -> Result<Initialize<common::HashedFile>, super::MissingFilename> {
         let init_hash = hashing::filename_hash(self, meta);
 
-        let hashed_path = format!("setup_python_{init_hash}.dist").into();
-        let unhashed_path = self.python_build_file_path.path().into();
-        let filename = self.python_build_file_path.filename()?;
-        let python_build_file_path = common::HashedFile::new(hashed_path, unhashed_path, filename);
+        // hash the sif
+        let hashed_path = format!("setup_sif_{init_hash}.dist").into();
+        let unhashed_path = self.sif.path().into();
+        let filename = self.sif.filename()?;
+        let sif = common::HashedFile::new(hashed_path, unhashed_path, filename);
 
         // hashed required files
         let required_files = self
             .required_files
             .iter()
             .enumerate()
             .map(|(idx, init_file)| {
@@ -152,59 +151,61 @@
                     unhashed_path,
                     filename,
                 ))
             })
             .collect::<Result<Vec<_>, super::MissingFilename>>()?;
 
         let init = Initialize {
-            python_build_file_path,
+            sif,
             required_files,
+            required_mounts: self.required_mounts.clone(),
         };
 
         Ok(init)
     }
 }
 
 #[cfg(feature = "cli")]
 impl Initialize<common::HashedFile> {
-    pub(super) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
-        files.push(self.python_build_file_path.as_sendable(is_user));
+    pub(crate) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
+        files.push(self.sif.as_sendable(is_user));
 
         self.required_files
             .iter()
             .for_each(|hashed_file| files.push(hashed_file.as_sendable(is_user)));
     }
 }
 
-#[derive(Debug, Clone, Deserialize, Serialize, Constructor, getset::Getters)]
+#[derive(Debug, Clone, Deserialize, Serialize, Constructor, Getters)]
 #[serde(deny_unknown_fields)]
-/// specification for a python job
+/// specification for an apptainer job
 pub struct Job<FILE> {
     #[getset(get = "pub(crate)")]
-    pub(super) name: String,
-    #[serde(rename = "file")]
-    #[getset(get = "pub(crate)")]
-    pub(super) python_job_file: FILE,
+    name: String,
     #[serde(default = "Default::default")]
     #[getset(get = "pub(crate)")]
-    pub(super) required_files: Vec<FILE>,
+    /// files required for the execution of this job
+    pub required_files: Vec<FILE>,
     /// slurm configuration. This level of information will override the defeaults at the outer
     /// most level of the configuration
+    #[getset(get = "pub(crate)")]
     slurm: Option<super::Slurm>,
 }
 
 #[cfg(feature = "cli")]
 impl Job<common::File> {
     pub(crate) fn hashed(
         &self,
         job_idx: usize,
         meta: &super::Meta,
     ) -> Result<Job<common::HashedFile>, super::MissingFilename> {
+        //
+        // for each job ...
+        //
         let hash = hashing::filename_hash(self, meta);
-
         let required_files = self
             .required_files
             .iter()
             .enumerate()
             .map(|(file_idx, file)| {
                 //
                 // for each file in this job ...
@@ -217,34 +218,64 @@
                     hashed_path,
                     unhashed_path,
                     filename,
                 ))
             })
             .collect::<Result<Vec<_>, super::MissingFilename>>()?;
 
-        let hashed_path = format!("{hash}_python_run.dist").into();
-        let unhashed_path = self.python_job_file.path().into();
-        let filename = self.python_job_file.filename()?;
-        let python_job_file = common::HashedFile::new(hashed_path, unhashed_path, filename);
-
         // assemble the new files into a new job
         let job = Job {
             name: self.name().to_string(),
-            python_job_file,
             required_files,
             slurm: self.slurm.clone(),
         };
 
         Ok(job)
     }
 }
-
 #[cfg(feature = "cli")]
 impl Job<common::HashedFile> {
     pub(crate) fn sendable_files(&self, is_user: bool, files: &mut Vec<FileMetadata>) {
-        files.push(self.python_job_file.as_sendable(is_user));
-
         self.required_files
             .iter()
             .for_each(|hashed_file| files.push(hashed_file.as_sendable(is_user)));
     }
 }
+
+#[test]
+fn hash_not_same() {
+    let namespace = "common_namespace".to_string();
+    let inner_caps: Vec<String> = vec![];
+    let caps =
+        super::requirements::Requirements::<super::requirements::JobRequiredCaps>::from(inner_caps);
+
+    let meta_1 = super::Meta {
+        batch_name: "batch_01".into(),
+        namespace: namespace.clone(),
+        matrix: None,
+        capabilities: caps.clone(),
+    };
+
+    let meta_2 = super::Meta {
+        batch_name: "batch_02".into(),
+        namespace: namespace.clone(),
+        matrix: None,
+        capabilities: caps.clone(),
+    };
+
+    let initialize: Initialize<common::File> = Initialize {
+        sif: common::File::new_relative("some_path.sif"),
+        required_files: Vec::new(),
+        required_mounts: Vec::new(),
+    };
+
+    let jobs = Vec::new();
+
+    let desc = Description { initialize, jobs };
+
+    let hashed_1 = desc.hashed(&meta_1).unwrap();
+    let hashed_2 = desc.hashed(&meta_2).unwrap();
+
+    dbg!(&hashed_1, &hashed_2);
+
+    assert!(hashed_1.initialize.sif.hashed_path() != hashed_2.initialize.sif.hashed_path());
+}
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/config/requirements.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/config/requirements.rs`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 /// or capabilities that a compute node relies on.
 ///
 ///
 /// ## Example
 ///
 /// ```
 /// use distribute::requirements::Requirements;
+/// use distribute::requirements::JobRequiredCaps;
+///
 /// let job_capabilities = vec!["gpu", "apptainer"];
 ///
-/// let requirements : Requirements = Requirements::from(job_capabilities);
+/// let requirements : Requirements<JobRequiredCaps> = Requirements::from(job_capabilities);
 /// ```
 pub struct Requirements<T> {
     pub(crate) reqs: BTreeSet<Requirement>,
     #[serde(skip)]
     pub(crate) marker: std::marker::PhantomData<T>,
 }
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/error.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/error.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/kill.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/kill.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/node_status.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/node_status.rs`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Online(Version),
     #[display(fmt = "OFFLINE")]
     Offline,
 }
 
 /// check if nodes are online & what their current version of `distribute` is
 pub async fn node_status(args: cli::NodeStatus) -> Result<(), Error> {
-    let nodes_config = config::load_config::<config::Nodes>(&args.nodes_file)?;
+    let nodes_config = config::load_config::<config::Nodes>(&args.nodes_file, true)?;
 
     let mut results = Vec::new();
 
     for node in nodes_config.nodes {
         let c = tokio::net::TcpStream::connect(node.keepalive_addr())
             .await
             .map_err(|e| {
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/pause/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/pause/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/pause/unix.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/pause/unix.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/prelude.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/built.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/built.rs`

 * *Files 8% similar despite different names*

```diff
@@ -125,20 +125,20 @@
     async fn into_prepare_build_state(self) -> super::prepare_build::ClientPrepareBuildState {
         let ClientBuiltState {
             conn,
             working_dir,
             cancel_addr,
             ..
         } = self.state;
+
         debug!("moving client built -> prepare build");
-        #[allow(unused_mut)]
+
         let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
         super::prepare_build::ClientPrepareBuildState {
             conn,
             working_dir,
             cancel_addr,
         }
     }
 
@@ -150,19 +150,16 @@
             conn,
             working_dir,
             folder_state,
             cancel_addr,
         } = self.state;
         debug!("moving client built -> executing");
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         // dump all the files in the ./input directory
         let save_location = working_dir.input_folder();
 
         let extra = send_files::ExecutingReceiver {
             working_dir,
             run_info,
@@ -290,19 +287,16 @@
     async fn into_prepare_build_state(self) -> super::prepare_build::ServerPrepareBuildState {
         debug!(
             "moving {} server built -> prepare_build",
             self.state.common.node_meta
         );
         let ServerBuiltState { conn, common, .. } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         super::prepare_build::ServerPrepareBuildState { conn, common }
     }
 
     async fn into_send_files_state(
         self,
         run_info: server::pool_data::RunTaskInfo,
@@ -316,19 +310,16 @@
             conn,
             common,
             namespace,
             batch_name,
             job_identifier: _,
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         let job_name = run_info.task.name();
 
         let save_location = common
             .save_path
             .join(namespace)
             .join(batch_name)
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/compiling.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/compiling.rs`

 * *Files 4% similar despite different names*

```diff
@@ -144,19 +144,17 @@
         let ClientBuildingState {
             conn,
             working_dir,
             cancel_addr,
             ..
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         super::built::ClientBuiltState {
             conn,
             working_dir,
             folder_state,
             cancel_addr,
         }
@@ -166,19 +164,18 @@
         let ClientBuildingState {
             conn,
             working_dir,
             cancel_addr,
             ..
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
+
         super::prepare_build::ClientPrepareBuildState {
             conn,
             working_dir,
             cancel_addr,
         }
     }
 }
@@ -252,19 +249,17 @@
         let ServerBuildingState {
             conn,
             common,
             namespace,
             batch_name,
             job_identifier,
         } = self.state;
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
         super::built::ServerBuiltState {
             conn,
             common,
             namespace,
             batch_name,
             job_identifier,
@@ -275,19 +270,18 @@
         debug!(
             "moving {} server compiling -> prepare build",
             self.state.common.node_meta
         );
 
         let ServerBuildingState { conn, common, .. } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
+
         super::prepare_build::ServerPrepareBuildState { conn, common }
     }
 }
 
 #[derive(Serialize, Deserialize, Unwrap, Debug)]
 pub(crate) enum ServerMsg {}
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/executing.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/executing.rs`

 * *Files 2% similar despite different names*

```diff
@@ -175,46 +175,45 @@
             conn,
             working_dir,
             folder_state,
             cancel_addr,
             run_info,
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         let job_name = run_info.task.name().to_string();
 
         let extra = send_files::SenderFinalStore {
             working_dir,
             job_name,
             folder_state,
             cancel_addr,
+            node_meta: server::pool_data::NodeMetadata {
+                node_name: "SERVER".into(),
+                node_address: *conn.addr(),
+            },
         };
 
         ClientSendFilesState { conn, extra }
     }
 
     async fn into_prepare_build_state(self) -> super::prepare_build::ClientPrepareBuildState {
         let ClientExecutingState {
             conn,
             working_dir,
             cancel_addr,
             ..
         } = self.state;
         debug!("moving client executing -> prepare build");
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
         super::prepare_build::ClientPrepareBuildState {
             conn,
             working_dir,
             cancel_addr,
         }
     }
 }
@@ -300,14 +299,15 @@
                 // have any practical effect on anything - nothing in this jobset
                 // really matters anymore so we dont need to create a special cancellation notice
                 info!("sending scheduler message that the job has been finished");
 
                 let finish_msg = server::pool_data::FinishJob {
                     ident: self.state.job_identifier(),
                     job_name: self.state.run_info.task.name().to_string(),
+                    node_meta: self.state.common.node_meta.clone(),
                 };
 
                 let mark_finished_msg = server::JobRequest::FinishJob(finish_msg);
                 scheduler_tx
                     .send(mark_finished_msg)
                     .await
                     .ok()
@@ -372,19 +372,16 @@
         let ServerExecutingState {
             conn,
             common,
             save_location,
             run_info,
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         let extra = send_files::ReceiverFinalStore { common, run_info };
 
         ServerSendFilesState {
             conn,
             save_location,
             extra,
@@ -394,19 +391,16 @@
     async fn into_prepare_build_state(self) -> super::prepare_build::ServerPrepareBuildState {
         debug!(
             "moving {} server executing -> prepare build",
             self.state.common.node_meta
         );
         let ServerExecutingState { conn, common, .. } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         super::prepare_build::ServerPrepareBuildState { conn, common }
     }
 
     pub(crate) fn node_name(&self) -> &str {
         &self.state.common.node_meta.node_name
     }
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,20 @@
 
 impl<StateMarker, T> Machine<StateMarker, transport::Connection<T>> {
     pub(crate) fn into_inner(self) -> transport::Connection<T> {
         self.state
     }
 }
 
+impl UninitServer {
+    pub(crate) fn node_meta(&self) -> &pool_data::NodeMetadata {
+        &self.state.common.node_meta
+    }
+}
+
 impl<T> SendFilesServer<T> {
     pub(crate) fn into_connection(self) -> transport::Connection<send_files::ServerMsg> {
         self.state.conn
     }
 }
 
 pub(crate) enum Either<T, V> {
@@ -232,7 +238,24 @@
             errored_jobs,
         );
 
         // tx here is a cancellation handle
         (tx, common)
     }
 }
+
+#[allow(unused_variables)]
+async fn assert_conn_empty<TX, RX>(conn: &mut transport::Connection<TX>) 
+where
+    TX: Serialize + transport::AssociatedMessage<Receive = RX>,
+    RX: serde::de::DeserializeOwned,
+{
+    #[cfg(test)] 
+    if conn.bytes_left().await != 0 {
+        error!(
+            "connection was not empty - this is guaranteed to cause error in following steps!"
+        );
+        panic!(
+            "connection was not empty - this is guaranteed to cause error in following steps!"
+        );
+    }
+}
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/prepare_build.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/prepare_build.rs`

 * *Files 14% similar despite different names*

```diff
@@ -57,16 +57,16 @@
         }
 
         let msg = self.state.conn.receive_data().await;
         let msg: ServerMsg = throw_error_with_self!(msg, self);
 
         let job: pool_data::BuildTaskInfo = msg.unwrap_initialize_job();
 
-        let compiling_state = self.into_send_files_state(job).await;
-        let machine = Machine::from_state(compiling_state);
+        let send_files_compiling_state = self.into_send_files_state(job).await;
+        let machine = Machine::from_state(send_files_compiling_state);
         Ok(machine)
     }
 
     pub(crate) fn into_uninit(self) -> Machine<Uninit, ClientUninitState> {
         let ClientPrepareBuildState {
             conn,
             working_dir,
@@ -90,19 +90,16 @@
         debug!("moving client prepare build -> send_files (compiling)");
         let ClientPrepareBuildState {
             conn,
             working_dir,
             cancel_addr,
         } = self.state;
 
-        #[allow(unused_mut)]
         let mut conn = conn.update_state();
-
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        super::assert_conn_empty(&mut conn).await;
 
         // TODO: have better function to generate this signature
         let save_location = working_dir.initial_files_folder();
 
         let extra = send_files::BuildingReceiver {
             working_dir,
             cancel_addr,
@@ -196,28 +193,25 @@
         let batch_name = &build_info.batch_name;
         let job_identifier = &build_info.identifier;
         debug!(
             "moving {} server prepare build -> send_files (building) for job set name {batch_name} (ident: {job_identifier})",
             self.state.common.node_meta
         );
         let ServerPrepareBuildState { conn, common } = self.state;
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
         let extra = send_files::BuildingSender { common, build_info };
 
         send_files::SenderState { conn, extra }
     }
 }
 
 #[derive(Serialize, Deserialize, Unwrap)]
-// TODO: also need to send full information to rebuild the next state if required
 pub(crate) enum ServerMsg {
     InitializeJob(pool_data::BuildTaskInfo),
 }
 
 #[derive(Debug)]
 enum FlatServerMsg {}
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 mod receiver;
 mod sender;
 
 use super::Machine;
 use crate::prelude::*;
+use crate::server::pool_data::NodeMetadata;
 
 pub(crate) use receiver::{
     BuildingReceiver, ExecutingReceiver, Nothing, ReceiverFinalStore, ReceiverState,
 };
 pub(crate) use sender::{
     BuildingSender, ExecutingSender, FlatFileList, SenderFinalStore, SenderState,
 };
@@ -22,14 +23,22 @@
 pub(crate) trait NextState {
     type Next;
     type Marker;
 
     fn next_state(self) -> Self::Next;
 }
 
+pub(crate) trait SendLogging {
+    fn job_identifier(&self) -> JobSetIdentifier;
+    fn namespace(&self) -> &str;
+    fn batch_name(&self) -> &str;
+    fn job_name(&self) -> &str;
+    fn node_meta(&self) -> &NodeMetadata;
+}
+
 #[derive(thiserror::Error, Debug, From)]
 pub(crate) enum ClientError {
     #[error("{0}")]
     TcpConnection(error::TcpConnection),
 }
 
 #[derive(thiserror::Error, Debug, From)]
@@ -127,14 +136,15 @@
     let client_conn = transport::Connection::from_connection(client_conn);
 
     let extra = SenderFinalStore {
         working_dir: base_dir.clone(),
         job_name: "test job name".into(),
         folder_state: client::BindingFolderState::new(),
         cancel_addr,
+        node_meta: NodeMetadata::by_name("SERVER")
     };
 
     let client_state = SenderState {
         conn: client_conn,
         extra,
     };
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/receiver.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/receiver.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 use tokio::io::AsyncWriteExt;
 
 use super::super::built::{self};
 use super::super::uninit::{self, ClientUninitState};
 use super::super::{UninitClient, UninitServer};
 use super::NextState;
-use super::{ClientMsg, SendFiles, ServerError, ServerMsg};
+use super::{ClientMsg, SendFiles, SendLogging, ServerError, ServerMsg};
 
 // in the job execution process, this is the server
 pub(crate) struct ReceiverState<T> {
     pub(crate) conn: transport::Connection<ServerMsg>,
     /// where the results of the job should be stored
     pub(crate) save_location: PathBuf,
     pub(crate) extra: T,
@@ -20,22 +20,14 @@
 
 /// additional state used when performing file transfer
 pub(crate) struct ReceiverFinalStore {
     pub(crate) run_info: server::pool_data::RunTaskInfo,
     pub(crate) common: super::super::Common,
 }
 
-pub(crate) trait SendLogging {
-    fn job_identifier(&self) -> JobSetIdentifier;
-    fn namespace(&self) -> &str;
-    fn batch_name(&self) -> &str;
-    fn job_name(&self) -> &str;
-    fn node_meta(&self) -> &NodeMetadata;
-}
-
 impl SendLogging for ReceiverFinalStore {
     fn job_identifier(&self) -> JobSetIdentifier {
         self.run_info.identifier
     }
 
     fn namespace(&self) -> &str {
         &self.run_info.namespace
@@ -70,22 +62,15 @@
             common, run_info, ..
         } = extra;
 
         let namespace = run_info.namespace;
         let batch_name = run_info.batch_name;
         let job_identifier = run_info.identifier;
 
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
-
-        //#[cfg(test)]
-        //{
-        //    info!("checking for remaining bytes on server side...");
-        //    assert!(conn.bytes_left().await == 0);
-        //}
+        let conn = conn.update_state();
 
         built::ServerBuiltState {
             conn,
             common,
             namespace,
             batch_name,
             job_identifier,
@@ -365,15 +350,17 @@
                     writer.flush().await.unwrap();
                 }
                 ClientMsg::FinishFiles => {
                     // first, tell the scheduler that this job has finished
                     let finish_msg = server::pool_data::FinishJob {
                         ident: self.state.extra.job_identifier(),
                         job_name: self.state.extra.job_name().to_string(),
+                        node_meta: self.state.extra.node_meta().clone(),
                     };
+
                     if let Err(_e) = scheduler_tx
                         .send(server::pool_data::JobRequest::FinishJob(finish_msg))
                         .await
                     {
                         error!(
                             "scheduler is down - cannot transmit that job {} has finished on {}",
                             self.state.extra.job_name(),
@@ -382,26 +369,29 @@
                         panic!(
                             "scheduler is down - cannot transmit that job {} has finished on {}",
                             self.state.extra.job_name(),
                             self.state.extra.node_meta()
                         );
                     }
 
+                    super::super::assert_conn_empty(&mut self.state.conn).await;
+
                     // we are now done receiving files
                     let built_state = self.state.next_state();
                     let machine = Machine::from_state(built_state);
                     return Ok(machine);
                 }
             }
 
             let tmp = self
                 .state
                 .conn
                 .transport_data(&ServerMsg::ReceivedFile)
                 .await;
+
             throw_error_with_self!(tmp, self);
         }
     }
 }
 
 impl Machine<SendFiles, ReceiverState<ReceiverFinalStore>> {
     pub(crate) fn into_uninit(self) -> (UninitServer, server::pool_data::RunTaskInfo) {
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/send_files/sender.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/send_files/sender.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,69 @@
 use super::Machine;
 use crate::prelude::*;
 
+use crate::server::pool_data::NodeMetadata;
 use client::utils;
 
 use super::super::built::{Built, ClientBuiltState};
 use super::super::uninit::ClientUninitState;
 use super::super::UninitClient;
 use super::super::UninitServer;
-use super::{ClientError, ClientMsg, NextState, SendFiles, ServerMsg, LARGE_FILE_BYTE_THRESHOLD};
+use super::{
+    ClientError, ClientMsg, NextState, SendFiles, SendLogging, ServerMsg, LARGE_FILE_BYTE_THRESHOLD,
+};
 use crate::client::execute::FileMetadata;
 use protocol::uninit::ServerUninitState;
 
 // in the job execution process, this is the client
 pub(crate) struct SenderState<T> {
     pub(crate) conn: transport::Connection<ClientMsg>,
     pub(crate) extra: T,
 }
 
 pub(crate) trait FileSender {
-    fn job_name(&self) -> &str;
     fn files_to_send(&self) -> Box<dyn Iterator<Item = FileMetadata> + Send>;
 }
 
 /// additional state for transporting final data from a job run to the server
 pub(crate) struct SenderFinalStore {
     pub(crate) job_name: String,
     pub(crate) folder_state: client::BindingFolderState,
     pub(crate) cancel_addr: SocketAddr,
     pub(crate) working_dir: WorkingDir,
+    // does not really matter, here for the interface mostly
+    pub(crate) node_meta: NodeMetadata,
 }
 
 impl FileSender for SenderFinalStore {
-    fn job_name(&self) -> &str {
-        &self.job_name
-    }
-
     fn files_to_send(&self) -> Box<dyn Iterator<Item = FileMetadata> + Send> {
         let folder_files_to_send = self.working_dir.distribute_save_folder();
         let files = utils::read_folder_files(&folder_files_to_send);
         Box::new(files.into_iter().skip(1))
     }
 }
 
+impl SendLogging for SenderFinalStore {
+    fn job_identifier(&self) -> JobSetIdentifier {
+        JobSetIdentifier::None
+    }
+    fn namespace(&self) -> &str {
+        "UNKNOWN"
+    }
+    fn batch_name(&self) -> &str {
+        "UNKNOWN"
+    }
+    fn job_name(&self) -> &str {
+        &self.job_name
+    }
+    fn node_meta(&self) -> &NodeMetadata {
+        &self.node_meta
+    }
+}
+
 impl NextState for SenderState<SenderFinalStore> {
     type Next = ClientBuiltState;
     type Marker = Built;
 
     fn next_state(self) -> Self::Next {
         info!("moving client send files -> built");
         let SenderState { conn, extra, .. } = self;
@@ -53,49 +71,41 @@
         let SenderFinalStore {
             working_dir,
             folder_state,
             cancel_addr,
             ..
         } = extra;
 
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
-
-        // TODO: find how to include this in non-async code
-        //
-        //#[cfg(test)]
-        //assert!(conn.bytes_left().await == 0);
+        let conn = conn.update_state();
 
         ClientBuiltState {
             conn,
             working_dir,
             folder_state,
             cancel_addr,
         }
     }
 }
 
 /// state for a simple list of files to transfer
 pub(crate) struct FlatFileList {
     pub(crate) files: Vec<FileMetadata>,
+    pub(crate) node_meta: NodeMetadata,
 }
 
 impl NextState for SenderState<FlatFileList> {
     type Next = transport::Connection<ClientMsg>;
     type Marker = ();
 
     fn next_state(self) -> Self::Next {
         self.conn
     }
 }
 
 impl FileSender for FlatFileList {
-    fn job_name(&self) -> &str {
-        "user_file_send"
-    }
     fn files_to_send(&self) -> Box<dyn Iterator<Item = FileMetadata> + Send> {
         warn!("enumerating files (flat send) and their destinations");
 
         for file in self.files.iter() {
             debug!(
                 "{} -> {}",
                 file.absolute_file_path.display(),
@@ -103,14 +113,32 @@
             );
         }
 
         Box::new(self.files.clone().into_iter())
     }
 }
 
+impl SendLogging for FlatFileList {
+    fn job_identifier(&self) -> JobSetIdentifier {
+        JobSetIdentifier::None
+    }
+    fn namespace(&self) -> &str {
+        "UNKNOWN"
+    }
+    fn batch_name(&self) -> &str {
+        "UNKNOWN"
+    }
+    fn job_name(&self) -> &str {
+        "UNKNOWN"
+    }
+    fn node_meta(&self) -> &NodeMetadata {
+        &self.node_meta
+    }
+}
+
 /// sending files to be used in the compilation process
 pub(crate) struct BuildingSender {
     pub(crate) common: protocol::Common,
     pub(crate) build_info: server::pool_data::BuildTaskInfo,
 }
 
 impl NextState for SenderState<BuildingSender> {
@@ -136,18 +164,14 @@
             batch_name,
             job_identifier,
         }
     }
 }
 
 impl FileSender for BuildingSender {
-    fn job_name(&self) -> &str {
-        "building_file_send"
-    }
-
     fn files_to_send(&self) -> Box<dyn Iterator<Item = FileMetadata> + Send> {
         let sendable_files = self.build_info.init.sendable_files(false);
         warn!("enumerating files (BUILDING) and their destinations");
 
         for file in sendable_files.iter() {
             debug!(
                 "{} -> {}",
@@ -156,14 +180,32 @@
             );
         }
 
         Box::new(sendable_files.into_iter())
     }
 }
 
+impl SendLogging for BuildingSender {
+    fn job_identifier(&self) -> JobSetIdentifier {
+        self.build_info.identifier
+    }
+    fn namespace(&self) -> &str {
+        &self.build_info.namespace
+    }
+    fn batch_name(&self) -> &str {
+        &self.build_info.batch_name
+    }
+    fn job_name(&self) -> &str {
+        "BUILDING"
+    }
+    fn node_meta(&self) -> &NodeMetadata {
+        &self.common.node_meta
+    }
+}
+
 /// sending files to be used in the compilation process
 pub(crate) struct ExecutingSender {
     pub(crate) common: protocol::Common,
     pub(crate) run_info: server::pool_data::RunTaskInfo,
     // where to dump the files that are output from the job *AFTER* the
     // job finishes.
     pub(crate) save_location: PathBuf,
@@ -189,34 +231,53 @@
             save_location,
             run_info,
         }
     }
 }
 
 impl FileSender for ExecutingSender {
-    fn job_name(&self) -> &str {
-        "building_file_send"
-    }
-
     fn files_to_send(&self) -> Box<dyn Iterator<Item = FileMetadata> + Send> {
         Box::new(self.run_info.task.sendable_files(false).into_iter())
     }
 }
 
+impl SendLogging for ExecutingSender {
+    fn job_identifier(&self) -> JobSetIdentifier {
+        self.run_info.identifier
+    }
+    fn namespace(&self) -> &str {
+        &self.run_info.namespace
+    }
+    fn batch_name(&self) -> &str {
+        &self.run_info.batch_name
+    }
+    fn job_name(&self) -> &str {
+        &self.run_info.task.name()
+    }
+    fn node_meta(&self) -> &NodeMetadata {
+        &self.common.node_meta
+    }
+}
+
 impl<T, NEXT, MARKER> Machine<SendFiles, SenderState<T>>
 where
-    T: FileSender,
+    T: FileSender + SendLogging,
     SenderState<T>: NextState<Marker = MARKER, Next = NEXT>,
     MARKER: Default,
 {
     /// read and send all files in the ./distribute_save folder that the job has left
     ///
     /// if there is an error reading a file, that file will be logged but not sent. The
     /// only possible error from this function is if the TCP connection is cut.
-    #[instrument(skip(self), fields(job_name=self.state.extra.job_name()))]
+    #[instrument(skip(self), fields(
+        job_name=self.state.extra.job_name(),
+        node_meta=%self.state.extra.node_meta(),
+        namespace=self.state.extra.namespace(),
+        batch_name=self.state.extra.batch_name(),
+    ))]
     pub(crate) async fn send_files(mut self) -> Result<Machine<MARKER, NEXT>, (Self, ClientError)> {
         let job_name = self.state.extra.job_name();
         let files_to_send = self.state.extra.files_to_send();
 
         for metadata in files_to_send {
             // remove leading directories up until (and including) distribute_save
 
@@ -308,14 +369,16 @@
         // tell the server we are done sending files and we should transition to the next state
         info!("done sending files - transitioning to next state");
 
         let msg = ClientMsg::FinishFiles;
         let tmp = self.state.conn.transport_data(&msg).await;
         throw_error_with_self!(tmp, self);
 
+        super::super::assert_conn_empty(&mut self.state.conn).await;
+
         let next_state = self.state.next_state();
         let machine = Machine::from_state(next_state);
         Ok(machine)
     }
 }
 
 impl Machine<SendFiles, SenderState<SenderFinalStore>> {
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/protocol/uninit.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/protocol/uninit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -123,19 +123,17 @@
 
     async fn into_prepare_build_state(self) -> super::prepare_build::ClientPrepareBuildState {
         let ClientUninitState {
             conn,
             working_dir,
             cancel_addr,
         } = self.state;
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
         debug!("moving client uninit -> prepare build");
         super::prepare_build::ClientPrepareBuildState {
             conn,
             working_dir,
             cancel_addr,
         }
@@ -217,19 +215,17 @@
 
     async fn into_prepare_build_state(self) -> super::prepare_build::ServerPrepareBuildState {
         debug!(
             "moving {} server uninit -> prepare build",
             self.state.common.node_meta
         );
         let ServerUninitState { conn, common } = self.state;
-        #[allow(unused_mut)]
-        let mut conn = conn.update_state();
 
-        #[cfg(test)]
-        assert!(conn.bytes_left().await == 0);
+        let mut conn = conn.update_state();
+        super::assert_conn_empty(&mut conn).await;
 
         super::prepare_build::ServerPrepareBuildState { conn, common }
     }
 
     /// update the underlying TCP connection that the state machine will use
     ///
     /// This method *must* be called if there was an error with the previous TCP
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/pull.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/pull.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 use std::io::Write;
 use std::net::SocketAddr;
 use std::path::Path;
 
 /// execute a query to pull files from a head node / server
 pub async fn pull(args: cli::Pull) -> Result<(), Error> {
     let config: config::Jobs<config::common::File> =
-        config::load_config(&args.job_file).map_err(error::PullErrorLocal::from)?;
+        config::load_config(&args.job_file, true).map_err(error::PullErrorLocal::from)?;
 
     let req = match args.filter {
         Some(cli::RegexFilter::Include { include }) => {
             validate_regex(&include)?;
             transport::PullFileRequest::new(
                 include,
                 true,
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/run_local.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/run_local.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 /// Internally, this does not use the same machinery as the normal execution of apptainer jobs, so
 /// this needs to be tested separately.
 pub async fn run_local(args: cli::Run) -> Result<(), RunErrorLocal> {
     let working_dir = WorkingDir::from(args.save_dir.clone());
 
     create_required_dirs(&args, &working_dir).await?;
 
-    let config = config::load_config::<config::Jobs<config::common::File>>(&args.job_file)?;
+    let config = config::load_config::<config::Jobs<config::common::File>>(&args.job_file, true)?;
 
     let apptainer_config = match config {
         config::Jobs::Apptainer(app) => app,
         config::Jobs::Python(_) => return Err(RunErrorLocal::OnlyApptainer),
     };
 
     let mut state = client::execute::BindingFolderState::new();
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/job_pool.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/job_pool.rs`

 * *Files 9% similar despite different names*

```diff
@@ -20,38 +20,43 @@
 {
     pub(super) fn spawn(mut self) -> JoinHandle<()> {
         tokio::task::spawn(async move {
             while let Some(new_req) = self.receive_requests.recv().await {
                 match new_req {
                     JobRequest::FinishJob(finish) => {
                         info!(
+                            node_meta = %finish.node_meta,
                             "marking a finished job for {} ({})",
                             finish.job_name, finish.ident
                         );
                         self.remaining_jobs
                             .finish_job(finish.ident, &finish.job_name);
                     }
                     // we want a new job from the scheduler
                     JobRequest::NewJob(new_req) => {
-                        debug!("a node has asked for a new job");
+                        debug!(node_meta = %new_req.node_meta, "a node has asked for a new job");
                         // if we are requesting a new job -not- right after building a job
 
                         let new_task: JobResponse = self.remaining_jobs.fetch_new_task(
                             new_req.initialized_job,
                             new_req.capabilities,
                             &new_req.build_failures,
-                            new_req.node_meta,
+                            new_req.node_meta.clone(),
                         );
+
+                        // log all the paths, ensure they exist
+                        new_task.enumerate_paths(&new_req.node_meta);
+
                         new_req.tx.send(new_task).ok().unwrap();
                     }
                     // a job failed to execute on the node
                     JobRequest::DeadNode(pending_job) => {
-                        debug!("a node has died for now, the job is returning to the scheduler");
+                        debug!(node_meta = %pending_job.node_meta, "a node has died for now, the job is returning to the scheduler");
                         self.remaining_jobs
-                            .add_job_back(pending_job.task, pending_job.identifier);
+                            .add_job_back(pending_job.task.task, pending_job.task.identifier);
 
                         continue;
                     }
                     // the server got a request to add a new job set
                     JobRequest::AddJobSet(set) => {
                         info!("added new job set `{}` to scheduler", set.batch_name());
                         if let Err(e) = self.remaining_jobs.insert_new_batch(set) {
@@ -104,14 +109,16 @@
                             cancel_query
                                 .cancel_batch
                                 .send(CancelResult::BatchNameMissing)
                                 .ok();
                         }
                     }
                     JobRequest::MarkBuildFailure(failure) => {
+                        info!(node_meta = %failure.node_meta, "marking job set as build failure on node");
+
                         self.remaining_jobs
                             .mark_build_failure(failure.ident, self.total_nodes);
                     }
                 };
                 //
             }
         })
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/matrix.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/matrix.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/mod.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 use tokio::sync::{broadcast, mpsc};
 
 #[cfg(feature = "cli")]
 /// start a server (head node) for the execution of `distribute`
 pub async fn server_command(server: cli::Server) -> Result<(), Error> {
     debug!("starting server");
 
-    let nodes_config = config::load_config::<config::Nodes>(&server.nodes_file)?;
+    let nodes_config = config::load_config::<config::Nodes>(&server.nodes_file, true)?;
     debug!("finished loading nodes config");
 
     if server.save_path.exists() && server.clean_output {
         std::fs::remove_dir_all(&server.save_path).map_err(|e| {
             error::ServerError::from(error::RemoveDirError::new(e, server.save_path.clone()))
         })?;
     }
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/node.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/node.rs`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,17 @@
 
         let execute = match send_execute_files.send_files().await {
             Ok(execute) => execute,
             Err((send_files_err_state, err)) => {
                 let (uninit, run_task_info) = send_files_err_state.into_uninit();
 
                 // return the task to the scheduler
-                let return_msg = server::JobRequest::DeadNode(run_task_info);
+                let dead_node =
+                    server::pool_data::DeadNode::new(run_task_info, uninit.node_meta().clone());
+                let return_msg = server::JobRequest::DeadNode(dead_node);
                 scheduler_tx
                     .send(return_msg)
                     .await
                     .ok()
                     .expect("scheduler is offine - irrecoverable error");
 
                 return Err((uninit, err.into()));
@@ -124,15 +126,17 @@
                 "{} error executing the job: {}, returning the job back to scheduler",
                 execute.node_name(),
                 err
             );
 
             let (uninit, run_task_info) = execute.into_uninit();
 
-            let return_msg = server::JobRequest::DeadNode(run_task_info);
+            let dead_node =
+                server::pool_data::DeadNode::new(run_task_info, uninit.node_meta().clone());
+            let return_msg = server::JobRequest::DeadNode(dead_node);
             scheduler_tx
                 .send(return_msg)
                 .await
                 .ok()
                 .expect("scheduler is offine - irrecoverable error");
 
             return Err((uninit, err.into()));
@@ -158,15 +162,17 @@
 
             info!("{} adding job `{}` from `{}` back to scheduler since it failed to send its files previously", 
                 node_name,
                 job_name,
                 run_task_info.batch_name,
             );
 
-            let return_msg = server::JobRequest::DeadNode(run_task_info);
+            let dead_node =
+                server::pool_data::DeadNode::new(run_task_info, uninit.node_meta().clone());
+            let return_msg = server::JobRequest::DeadNode(dead_node);
             scheduler_tx
                 .send(return_msg)
                 .await
                 .ok()
                 .expect("scheduler is offine - irrecoverable error");
 
             //
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/schedule.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/schedule.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server/user_conn.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server/user_conn.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/server_status.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/server_status.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/slurm.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/slurm.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 const CURRENT_DUR_BASH: &[u8] = br#"DIR="$(cd "$(dirname "$0")" && pwd)""#;
 
 /// convert a distribute job to a slurm job
 pub fn slurm(args: cli::Slurm) -> Result<(), error::Slurm> {
     //
     // load the config files
     //
-    let jobs = config::load_config::<config::Jobs<config::common::File>>(&args.jobs)?;
+    let jobs = config::load_config::<config::Jobs<config::common::File>>(&args.jobs, true)?;
 
     if jobs.len_jobs() == 0 {
         return Err(error::Slurm::NoJobs);
     }
 
     // ensure that there are no duplicate job names
     crate::add::check_has_duplicates(&jobs.job_names())?;
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/template.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/template.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/src/transport.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/src/transport.rs`

 * *Files 4% similar despite different names*

```diff
@@ -150,70 +150,14 @@
         fmt.debug_struct("File")
             .field("file_name", &self.file_name)
             .field("file_bytes (length)", &self.file_bytes.len())
             .finish()
     }
 }
 
-//#[derive(Deserialize, Serialize, Clone, PartialEq, Eq)]
-//pub struct PythonJob {
-//    pub python_file: Vec<u8>,
-//    pub job_name: String,
-//    pub job_files: Vec<File>,
-//}
-//
-//impl fmt::Debug for PythonJob {
-//    fn fmt(&self, fmt: &mut fmt::Formatter<'_>) -> fmt::Result {
-//        fmt.debug_struct("PythonJob")
-//            .field("job_name", &self.job_name)
-//            .field("job_files", &self.job_files)
-//            .field("python_file (length)", &self.python_file.len())
-//            .finish()
-//    }
-//}
-//
-//#[derive(Deserialize, Serialize, Clone, PartialEq, Eq)]
-//pub struct ApptainerJob {
-//    pub job_name: String,
-//    pub job_files: Vec<File>,
-//}
-//
-//impl fmt::Debug for ApptainerJob {
-//    fn fmt(&self, fmt: &mut fmt::Formatter<'_>) -> fmt::Result {
-//        fmt.debug_struct("ApptainerJob")
-//            .field("job_name", &self.job_name)
-//            .field("job_files", &self.job_files)
-//            .finish()
-//    }
-//}
-//
-//#[derive(Clone, PartialEq, From, Debug, Serialize, Deserialize, Eq)]
-//pub(crate) enum JobOpt {
-//    Apptainer(ApptainerJob),
-//    Python(PythonJob),
-//}
-//
-//impl JobOpt {
-//    pub(crate) fn name(&self) -> &str {
-//        match &self {
-//            Self::Apptainer(x) => &x.job_name,
-//            Self::Python(x) => &x.job_name,
-//        }
-//    }
-//
-//    #[cfg(test)]
-//    pub(crate) fn placeholder_test_data() -> Self {
-//        transport::JobOpt::Python(transport::PythonJob {
-//            python_file: vec![],
-//            job_name: "test_job".into(),
-//            job_files: vec![],
-//        })
-//    }
-//}
-
 #[derive(Deserialize, Serialize, PartialEq, Eq, Display, Debug)]
 #[display(fmt = "{}.{}.{}", major, minor, patch)]
 pub struct Version {
     major: u16,
     minor: u16,
     patch: u16,
 }
@@ -255,14 +199,15 @@
 fn serialization_options() -> bincode::config::DefaultOptions {
     bincode::config::DefaultOptions::new()
 }
 
 #[derive(derive_more::From)]
 pub(crate) struct Connection<T> {
     conn: TcpStream,
+    addr: SocketAddr,
     _marker: std::marker::PhantomData<T>,
 }
 
 impl<T> fmt::Debug for Connection<T> {
     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
         write!(fmt, "connection transporting {} messages", stringify!(T))
     }
@@ -276,20 +221,22 @@
     pub(crate) async fn new(addr: SocketAddr) -> Result<Self, error::TcpConnection> {
         let conn = TcpStream::connect(addr)
             .await
             .map_err(error::TcpConnection::from)?;
 
         Ok(Self {
             conn,
+            addr,
             _marker: std::marker::PhantomData,
         })
     }
 
     pub(crate) fn from_connection(conn: TcpStream) -> Self {
         Self {
+            addr: conn.peer_addr().unwrap(),
             conn,
             _marker: std::marker::PhantomData,
         }
     }
 
     pub(crate) async fn transport_data(
         &mut self,
@@ -331,28 +278,32 @@
         Ok(())
     }
 
     pub(crate) fn update_state<TxNew>(self) -> Connection<TxNew> {
         let conn = self.conn;
         Connection {
             conn,
+            addr: self.addr,
             _marker: std::marker::PhantomData,
         }
     }
 
-    #[cfg(test)]
     /// determine how many bytes are remaining in the connection
     pub(crate) async fn bytes_left(&mut self) -> usize {
         let mut buffer = vec![0; 100];
         //let fut = read_buffer_bytes(&mut buffer, &mut self.conn);
         let fut = self.conn.read(&mut buffer[0..]);
         let buffer_length: Result<Result<usize, _>, _> =
             tokio::time::timeout(Duration::from_millis(500), fut).await;
         buffer_length.map(|x| x.unwrap_or(0)).unwrap_or(0)
     }
+
+    pub(crate) fn addr(&self) -> &SocketAddr {
+        &self.addr
+    }
 }
 
 /// serialize a `T` to bytes and send it through a TCP connection
 async fn transport<T: Serialize>(
     tcp_connection: &mut TcpStream,
     data: &T,
     is_keepalive: bool,
```

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-jobs-apptainer.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-jobs-apptainer.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-jobs-python.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-jobs-python.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/static/example-nodes.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/static/example-nodes.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local/run.py` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/apptainer_local.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/apptainer_local.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/cancel_job.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/cancel_job.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_deallocate_jobs.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_deallocate_jobs.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/check_pull.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/check_pull.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/tests/failed_keepalive.rs` & `distribute_compute_config-0.14.3/local_dependencies/distribute/tests/failed_keepalive.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/local_dependencies/distribute/update_python_version.sh` & `distribute_compute_config-0.14.3/local_dependencies/distribute/update_python_version.sh`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/README.md` & `distribute_compute_config-0.14.3/README.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/distribute_compute_config.pyi` & `distribute_compute_config-0.14.3/distribute_compute_config.pyi`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/Makefile` & `distribute_compute_config-0.14.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/make.bat` & `distribute_compute_config-0.14.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/source/api.rst` & `distribute_compute_config-0.14.3/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/source/conf.py` & `distribute_compute_config-0.14.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/source/example.rst` & `distribute_compute_config-0.14.3/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/docs/source/index.rst` & `distribute_compute_config-0.14.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/src/lib.rs` & `distribute_compute_config-0.14.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/src/validate_bindings.py` & `distribute_compute_config-0.14.3/src/validate_bindings.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/src/wrap.rs` & `distribute_compute_config-0.14.3/src/wrap.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.2/Cargo.lock` & `distribute_compute_config-0.14.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
  "quote",
  "rustc_version",
  "syn",
 ]
 
 [[package]]
 name = "distribute"
-version = "0.14.2"
+version = "0.14.3"
 dependencies = [
  "base16",
  "derive_more",
  "getset",
  "matrix-notify",
  "pyo3",
  "serde",
```

### Comparing `distribute_compute_config-0.14.2/PKG-INFO` & `distribute_compute_config-0.14.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distribute_compute_config
-Version: 0.14.2
+Version: 0.14.3
 Summary: 
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # pybind
 
 Python bindings to `distribute` for automated creation of configuration files
```

