# Comparing `tmp/daqp-0.4.1.tar.gz` & `tmp/daqp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daqp-0.4.1.tar", last modified: Fri Apr  7 15:49:37 2023, max compression
+gzip compressed data, was "daqp-0.5.0.tar", last modified: Tue Apr 11 07:57:35 2023, max compression
```

## Comparing `daqp-0.4.1.tar` & `daqp-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-07 15:49:36.000000 daqp-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-07 15:40:58.000000 daqp-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 15:49:37.131278 daqp-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-07 15:40:58.000000 daqp-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.127278 daqp-0.4.1/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/csrc/include/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/api.h
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/auxiliary.h
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/bnb.h
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/daqp.h
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/daqp_prox.h
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/factorization.h
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/types.h
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/include/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/csrc/src/
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/api.c
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/auxiliary.c
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/bnb.c
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/daqp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/daqp_prox.c
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/factorization.c
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-04-07 15:40:58.000000 daqp-0.4.1/csrc/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (123)   835898 2023-04-07 15:49:36.000000 daqp-0.4.1/daqp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:49:37.131278 daqp-0.4.1/daqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:49:36.000000 daqp-0.4.1/daqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 15:49:37.000000 daqp-0.4.1/daqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-07 15:40:58.000000 daqp-0.4.1/daqp.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-07 15:40:58.000000 daqp-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 15:49:37.131278 daqp-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-07 15:40:58.000000 daqp-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:57:35.121277 daqp-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 07:57:34.000000 daqp-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-11 07:46:13.000000 daqp-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 07:57:35.121277 daqp-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-11 07:46:13.000000 daqp-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:57:35.109277 daqp-0.5.0/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:57:35.117277 daqp-0.5.0/csrc/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/api.h
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/auxiliary.h
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/bnb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/daqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/daqp_prox.h
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/factorization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/include/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:57:35.117277 daqp-0.5.0/csrc/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/api.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/auxiliary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/bnb.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/daqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/daqp_prox.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/factorization.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-11 07:46:13.000000 daqp-0.5.0/csrc/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)   845258 2023-04-11 07:57:34.000000 daqp-0.5.0/daqp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:57:35.121277 daqp-0.5.0/daqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 07:57:35.000000 daqp-0.5.0/daqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 07:57:35.000000 daqp-0.5.0/daqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:57:35.000000 daqp-0.5.0/daqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:57:34.000000 daqp-0.5.0/daqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 07:57:35.000000 daqp-0.5.0/daqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-11 07:46:13.000000 daqp-0.5.0/daqp.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-11 07:46:13.000000 daqp-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 07:57:35.121277 daqp-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-11 07:46:13.000000 daqp-0.5.0/setup.py
```

### Comparing `daqp-0.4.1/LICENSE` & `daqp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/PKG-INFO` & `daqp-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daqp
-Version: 0.4.1
+Version: 0.5.0
 Summary: DAQP: A dual active-set QP solver
 Home-page: http://github.com/darnstrom/daqp
 Author: Daniel Arnström
 Author-email: daniel.arnstrom@liu.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daqp-0.4.1/README.md` & `daqp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/csrc/include/constants.h` & `daqp-0.5.0/csrc/include/constants.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #ifndef DAQP_CONSTANTS_H
 #define DAQP_CONSTANTS_H
 
+# ifdef __cplusplus
+extern "C" {
+# endif // ifdef __cplusplus
+
 #include <stddef.h>
 
 #define EMPTY_IND -1 
 #define NX work->n 
 #define N_CONSTR work->m 
 #define N_SIMPLE work->ms 
 #define DAQP_INF ((c_float)1e30)
@@ -77,9 +81,12 @@
 #define IS_SLACK_FIXED(x) (work->sense[x]&32)
 #define IS_SLACK_FREE(x) ((work->sense[x]&32)==0)
 #define SET_SLACK_FIXED(x) (work->sense[x]|=32)
 #define SET_SLACK_FREE(x) (work->sense[x]&=~32)
 
 #define IS_SIMPLE(x) (x < work->ms)
 
+# ifdef __cplusplus
+}
+# endif // ifdef __cplusplus
 
 #endif //ifndef DAQP_CONSTANTS_H
```

### Comparing `daqp-0.4.1/csrc/include/types.h` & `daqp-0.5.0/csrc/include/types.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #ifndef DAQP_TYPES_H
 # define DAQP_TYPES_H
 
+# ifdef __cplusplus
+extern "C" {
+# endif // ifdef __cplusplus
+
 #ifdef DAQP_SINGLE_PRECISION
 typedef float c_float;
 #else
 typedef double c_float;
 #endif
 
 typedef struct{
@@ -19,31 +23,29 @@
     // m  - total number of constraints
     // ms - number of simple bounds
     // blower = [lb; lbA];
     // bupper = [ub; ubA];
     // (The number of rows in A is hence m-ms)
 
     // sense define the state of the constraints 
-    // (active, immutable, upper/lower, soft). 
+    // (active, immutable, upper/lower, soft, binary).
 
     int n;
     int m;
     int ms;
 
     c_float* H;
     c_float* f;
 
     c_float* A;
     c_float* bupper;
     c_float* blower;
 
     int* sense; 
 
-    int* bin_ids;
-    int nb;
 }DAQPProblem;
 
 typedef struct{
     c_float primal_tol;
     c_float dual_tol;
     c_float zero_tol;
     c_float pivot_tol;
@@ -148,8 +150,12 @@
     // Settings
     DAQPSettings* settings;
 
     // BnB
     DAQPBnB* bnb;
 }DAQPWorkspace;
 
+# ifdef __cplusplus
+}
+# endif // ifdef __cplusplus
+
 #endif //ifndef DAQP_TYPES_H
```

### Comparing `daqp-0.4.1/csrc/include/utils.h` & `daqp-0.5.0/csrc/include/utils.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 #ifndef DAQP_UTILS_H
 # define DAQP_UTILS_H
+
+# ifdef __cplusplus
+extern "C" {
+# endif // ifdef __cplusplus
+
 #include "daqp.h"
 // Utils for transforming QP to LDP
 int update_ldp(const int mask, DAQPWorkspace *work);
 int update_Rinv(DAQPWorkspace *work);
 void update_M(DAQPWorkspace *work, const int mask);
 void update_v(c_float *f, DAQPWorkspace *work, const int mask);
 void update_d(DAQPWorkspace *work);
@@ -28,8 +33,12 @@
 
 
 void tic(DAQPtimer *timer);
 void toc(DAQPtimer *timer);
 double get_time(DAQPtimer *timer);
 #endif // PROFILING
 
+# ifdef __cplusplus
+}
+# endif // ifdef __cplusplus
+
 #endif //ifndef DAQP_UTILS_H
```

### Comparing `daqp-0.4.1/csrc/src/api.c` & `daqp-0.5.0/csrc/src/api.c`

 * *Files 5% similar despite different names*

```diff
@@ -64,32 +64,34 @@
         *setup_time = 0; // in case setup fails 
         tic(&timer);
     }
 #endif
     // Check if QP is well-posed
     //validate_QP(qp);
 
-    // Count number of soft constraints
+    // Count number of soft/binary constraints 
     // (to account for it in allocation)
-    int ns = 0;
-    for(int i = 0; i < qp->m ; i++)
+    int ns = 0, nb = 0;
+    for(int i = 0; i < qp->m ; i++){
         if(qp->sense[i] & SOFT) ns++;
+        if(qp->sense[i] & BINARY) nb++;
+    }
     // Setup workspace
     if(work->settings == NULL)
         allocate_daqp_settings(work);
     else
         own_settings = 0;
     allocate_daqp_workspace(work,qp->n,ns);
     errorflag = setup_daqp_ldp(work,qp);
     if(errorflag < 0){
         if(own_settings==0) work->settings = NULL;
         free_daqp_workspace(work);
         return errorflag;
     }
-    errorflag = setup_daqp_bnb(work,qp->bin_ids,qp->nb, ns);
+    errorflag = setup_daqp_bnb(work, nb, ns);
     if(errorflag < 0){
         if(own_settings==0) work->settings = NULL;
         free_daqp_workspace(work);
         return errorflag;
     }
     errorflag = activate_constraints(work);
     if(errorflag < 0){
@@ -160,28 +162,33 @@
     if(error_flag<0){
         free_daqp_ldp(work);
         return error_flag;
     }
     return 1;
 }
 
-int setup_daqp_bnb(DAQPWorkspace* work, int* bin_ids, int nb, int ns){
+int setup_daqp_bnb(DAQPWorkspace* work, int nb, int ns){
     if(nb > work->n) return EXIT_OVERDETERMINED_INITIAL;
     if((work->bnb == NULL) && (nb >0)){
         work->bnb= malloc(sizeof(DAQPBnB));
 
         work->bnb->nb = nb;
-        work->bnb->bin_ids = bin_ids;
+        // Detect which constraints are binary
+        work->bnb->bin_ids = malloc(nb*sizeof(int));
+        for(int i = 0, nadded = 0; nadded < nb; i++){
+            if(work->qp->sense[i] & BINARY)
+                work->bnb->bin_ids[nadded++] = i;
+        }
 
         // Setup tree
         work->bnb->tree= malloc((work->bnb->nb+1)*sizeof(DAQPNode));
-        work->bnb->tree_WS= malloc((work->n+ns+1)*(work->bnb->nb+1)*sizeof(int));
+        work->bnb->tree_WS= malloc((work->n+ns+1)*(nb+1)*sizeof(int));
         work->bnb->n_nodes = 0; 
         work->bnb->nWS= 0; 
-        work->bnb->fixed_ids= malloc((work->bnb->nb+1)*sizeof(int));
+        work->bnb->fixed_ids= malloc((nb+1)*sizeof(int));
     }
     return 1;
 }
 
 // Free data for LDP 
 void free_daqp_ldp(DAQPWorkspace *work){
     if(work->sense==NULL) return; // Already freed
@@ -308,21 +315,22 @@
         for(i=0;i<work->m;i++) 
             res->lam[i] = 0; 
         for(i=0;i<work->n_active;i++)
             res->lam[work->WS[i]] = work->lam_star[i];
     }
 
     // Shift back function value
-    if(work->v != NULL && (work->settings->eps_prox == 0 || work->Rinv != NULL)){ // Normal QP
+    if(work->v != NULL && (work->settings->eps_prox == 0
+                || work->Rinv != NULL || work->RinvD != NULL)){ // Normal QP
         res->fval = work->fval;
         for(i=0;i<work->n;i++) res->fval-=work->v[i]*work->v[i];
         res->fval *=0.5;
         if(work->settings->eps_prox != 0)
-        for(i=0;i<work->n;i++) // compensate for proximal iterations
-            res->fval+= work->settings->eps_prox*work->x[i]*work->x[i];
+            for(i=0;i<work->n;i++) // compensate for proximal iterations
+                res->fval+= work->settings->eps_prox*work->x[i]*work->x[i];
     }
     else if(work->qp != NULL && work->qp->f != NULL ){ // LP
         res->fval = 0;
         for(i=0;i<work->n;i++) res->fval+=work->qp->f[i]*work->x[i];
     }
 
     // info
```

### Comparing `daqp-0.4.1/csrc/src/auxiliary.c` & `daqp-0.5.0/csrc/src/auxiliary.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/csrc/src/bnb.c` & `daqp-0.5.0/csrc/src/bnb.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/csrc/src/daqp.c` & `daqp-0.5.0/csrc/src/daqp.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/csrc/src/daqp_prox.c` & `daqp-0.5.0/csrc/src/daqp_prox.c`

 * *Files 6% similar despite different names*

```diff
@@ -28,48 +28,48 @@
         else 
             ldp2qp_solution(work); // Get qp solution 
 
         if(eps==0) break; // No regularization -> no outer iterations
 
         // ** Check convergence **
         if(work->iterations==1){ // No changes to the working set 
-            tol_stat = (work->Rinv == NULL) ? eta*eps : eta/eps;
+            tol_stat = (work->Rinv == NULL && work->RinvD == NULL) ? eta*eps : eta/eps;
             for(i=0, diff= 0;i<nx;i++){ // ||x_old - x|| > eta  ?
                 diff= work->x[i] - work->xold[i];
                 if((diff> tol_stat) || (diff< -tol_stat)) break;
             }
             if(i==nx){
                 exitflag = EXIT_OPTIMAL; // Fix point reached
                 break;
             }
             // Take gradient step if LP (and the iterate is not constrained to a vertex)
-            if((work->Rinv == NULL)&&(work->n_active != NX)){
+            if((work->Rinv == NULL && work->RinvD ==NULL )&&(work->n_active != NX)){
                 if(gradient_step(work)==EMPTY_IND){
                     exitflag= EXIT_UNBOUNDED;
                     break;
                 }
             }
         }
         // For LPs, compute objective function value to detect progress
         // TODO: add paramters to settings
-        if(work->Rinv == NULL){
+        if(work->Rinv == NULL && work->RinvD == NULL){
             for(i=0, diff=best_fval;i<nx;i++)
                 diff-=work->qp->f[i]*work->x[i];
             if(diff<1e-10){
                 if(cycle_counter++ > 10) return EXIT_OPTIMAL; // assume fix point
             }
             else{ // Progress -> update objective function value
                 best_fval -=diff ;
                 cycle_counter=0;
             }
         }
 
         // ** Perturb problem **
         // Compute v = R'\(f-eps*x) (FWS Skipped if LP since R = I) 
-        if(work->Rinv== NULL){ 
+        if(work->Rinv== NULL && work->RinvD == NULL){ 
             eps*= (work->iterations==1) ? 10 : 0.9; // Adapt epsilon TODO: add to settings 
             eps = (eps > 1e3) ? 1e3 : eps; // TODO: add saturation option to settings
             for(i = 0; i<nx;i++) 
                 work->v[i] = work->qp->f[i]*eps-work->x[i];
         }
         else{
             for(i = 0; i<nx;i++) 
@@ -77,15 +77,15 @@
             update_v(work->v,work,0);
         }
         // Perturb RHS of constraints 
         update_d(work);
     }
     // Finalize results
     if(total_iter >= work->settings->iter_limit) exitflag = EXIT_ITERLIMIT; 
-    if(work->Rinv == NULL){
+    if(work->Rinv == NULL && work->RinvD == NULL){
         for(i = 0; i<work->n_active;i++) 
             work->lam_star[i]/=eps;// Rescale dual variables
     }
     work->iterations = total_iter;
     return exitflag;
 }
 // Gradient step
```

### Comparing `daqp-0.4.1/csrc/src/factorization.c` & `daqp-0.5.0/csrc/src/factorization.c`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/csrc/src/utils.c` & `daqp-0.5.0/csrc/src/utils.c`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,25 @@
     if(mask&UPDATE_Rinv){
         normalize_Rinv(work);
     }
 
     /** Update d **/
     if(mask&UPDATE_Rinv||mask&UPDATE_M||mask&UPDATE_v||mask&UPDATE_d){
 #ifndef DAQP_ASSUME_VALID
-        // Check for trivial infeasibility
+        c_float diff;
         for(int i =0;i<N_CONSTR;i++){
-            if((work->qp->bupper[i] - work->qp->blower[i])< -work->settings->primal_tol){
-                if(IS_IMMUTABLE(i))
-                    continue;
-                else
-                    return EXIT_INFEASIBLE;
+            if(IS_IMMUTABLE(i)) continue;
+            diff = work->qp->bupper[i] - work->qp->blower[i];
+            // Check for trivial infeasibility
+            if ( diff < -work->settings->primal_tol ){
+                return EXIT_INFEASIBLE;
             }
+            // Check for unmarked equality constraint (blower == bupper)
+            else if ( diff < work->settings->zero_tol )
+                work->sense[i] |= ACTIVE + IMMUTABLE;
         }
 #endif
         update_d(work);
     }
 
 
 #ifdef SOFT_WEIGHTS
@@ -87,23 +90,23 @@
     if(is_diagonal==1){
         work->RinvD = work->Rinv;
         work->Rinv = NULL;
         c_float Hi;
         i=0; disp=0;
         if(work->scaling != NULL){
             for(;i<N_SIMPLE;i++,disp+=n){ // Combine with settings scaling
-                Hi = work->qp->H[disp++];
+                Hi = work->qp->H[disp++]+work->settings->eps_prox;
                 if (Hi <= 0) return EXIT_NONCONVEX;
                 Hi = sqrt(Hi);
                 work->RinvD[i] = 1/Hi;
                 work->scaling[i] = Hi;
             }
         }
         for(;i<n;i++,disp+=n){
-            Hi = work->qp->H[disp++];
+            Hi = work->qp->H[disp++] + work->settings->eps_prox;
             if (Hi <= 0) return EXIT_NONCONVEX;
             Hi = sqrt(Hi);
             work->RinvD[i] = 1/Hi;
         }
         return 1;
     }
     // Make sure Rinv can be assinged if not diagonal
```

### Comparing `daqp-0.4.1/daqp.c` & `daqp-0.5.0/daqp.c`

 * *Files 1% similar despite different names*

```diff
@@ -1455,14 +1455,17 @@
 
 /* IterFinish.proto */
 static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* UnpackItemEndCheck.proto */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
 
+/* PyIntCompare.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, long intval, long inplace);
+
 /* BufferIndexError.proto */
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
@@ -1977,39 +1980,43 @@
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
+static const char __pyx_k_A_ptr[] = "A_ptr";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_nodes[] = "nodes";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_sense[] = "sense";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_solve[] = "solve";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
+static const char __pyx_k_bl_ptr[] = "bl_ptr";
 static const char __pyx_k_blower[] = "blower";
+static const char __pyx_k_bu_ptr[] = "bu_ptr";
 static const char __pyx_k_bupper[] = "bupper";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_asarray[] = "asarray";
 static const char __pyx_k_fortran[] = "fortran";
+static const char __pyx_k_lam_ptr[] = "lam_ptr";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_problem[] = "problem";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_daqp_pyx[] = "daqp.pyx";
 static const char __pyx_k_dual_tol[] = "dual_tol";
 static const char __pyx_k_eps_prox[] = "eps_prox";
 static const char __pyx_k_eta_prox[] = "eta_prox";
@@ -2022,14 +2029,15 @@
 static const char __pyx_k_zero_tol[] = "zero_tol";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_cycle_tol[] = "cycle_tol";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pivot_tol[] = "pivot_tol";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
+static const char __pyx_k_sense_ptr[] = "sense_ptr";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_abs_subopt[] = "abs_subopt";
 static const char __pyx_k_fval_bound[] = "fval_bound";
 static const char __pyx_k_iter_limit[] = "iter_limit";
 static const char __pyx_k_iterations[] = "iterations";
 static const char __pyx_k_primal_tol[] = "primal_tol";
@@ -2076,14 +2084,15 @@
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static PyObject *__pyx_n_s_A;
 static PyObject *__pyx_n_s_ASCII;
+static PyObject *__pyx_n_s_A_ptr;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
@@ -2105,15 +2114,17 @@
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_abs_subopt;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_asarray;
 static PyObject *__pyx_n_s_ascontiguousarray;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_bin_ids_cand;
+static PyObject *__pyx_n_s_bl_ptr;
 static PyObject *__pyx_n_s_blower;
+static PyObject *__pyx_n_s_bu_ptr;
 static PyObject *__pyx_n_s_bupper;
 static PyObject *__pyx_n_s_c;
 static PyObject *__pyx_n_u_c;
 static PyObject *__pyx_n_s_class;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_kp_s_contiguous_and_direct;
 static PyObject *__pyx_kp_s_contiguous_and_indirect;
@@ -2142,14 +2153,15 @@
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_info;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_iter_limit;
 static PyObject *__pyx_n_s_iterations;
 static PyObject *__pyx_n_s_lam;
+static PyObject *__pyx_n_s_lam_ptr;
 static PyObject *__pyx_n_s_m;
 static PyObject *__pyx_n_s_mA;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_ms;
 static PyObject *__pyx_n_s_n;
@@ -2181,14 +2193,15 @@
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_rel_subopt;
 static PyObject *__pyx_n_s_res;
 static PyObject *__pyx_n_s_rho_soft;
 static PyObject *__pyx_n_s_sense;
+static PyObject *__pyx_n_s_sense_ptr;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_settings;
 static PyObject *__pyx_n_s_setup_time;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_solve;
@@ -2312,15 +2325,16 @@
  * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
  *         double[:] bupper, double[:] blower=None, int[:] sense =None,
  *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4daqp_1solve(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_4daqp_1solve = {"solve", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4daqp_1solve, METH_VARARGS|METH_KEYWORDS, 0};
+static char __pyx_doc_4daqp_solve[] = "\n    Solve the quadratic program      minimize       0.5 x'*H*x + f' x\n                                    subject to   blower <= A x <= bupper\n    Example calls:\n    x, fval, exitflag, info = daqp.solve(H, f, A, bupper)\n    x, fval, exitflag, info = daqp.solve(H, f, A, bupper, blower)\n    x, fval, exitflag, info = daqp.solve(H, f, A, bupper, blower, sense)\n\n    Equality and binary constraints are supported (see information about sense below)\n\n    If bupper and blower have more elements than rows of A, the first elements of\n    bupper and bupper are interpreted as simple bounds.\n    For example\n        A = [[7.0 9.0]]\n        bupper = [2.0 3.0]\n        blower = [-4.0, -5.0]\n    is interpreted as\n        -4.0 <= x1 <= 2.0\n        -5.0 <= 7.0 x1 + 9.0 x2 <= 3.0.\n\n    Parameters\n    ---\n    H :\n        Cost matrix (should be positive definite).\n        For a singular cost matrix, e.g. for LPs, use a positive value for the setting eps_prox\n        (see information of how to change settings below)\n    f :\n        Cost vector.\n    A :\n        Linear constraint matrix.\n    bupper :\n        Upper bound on linear constraints.\n    blower:\n        Lower bound on linear constraints (default = -inf).\n    sense:\n        Integer array that determines constraint types. For example:\n          * 0  ->  Inequality constraint (default)\n          * 1  ->  Active inequality constraint (used as warm start)\n          * 5  ->  Equality constraint\n          * 8  ->  Soft constraint (allowed to be violated if necessary) \n          * 16 ->  Binary constraint (the upper or lower bound should hold with equality)\n    See <https://darnstrom.github.io/daqp/parameters>`_ for more information\n\n    Keyword arguments are used for settings. For example:\n       daqp.solve(H, f, A, bupper, blower, sense, primal_tol=1e-6, iter_limit=1000)\n    Available settings include:\n       * iter_limit : Maximum numer of allowed iterations\n       * primal_tol : Primal feas""ibility tolerance\n       * dual_tol   : Dual feasibility tolerance\n       * eps_pro x  : Regularization used for proximal-point iterations\n    See <https://darnstrom.github.io/daqp/parameters>`_ for all available settings.\n\n    Returns\n    -------\n    x :\n        Optimal primal solution.\n    fval :\n        Optimal cost.\n    exitflag :\n        Termination status; 1 signifies that an optimal solution was found.\n        See <https://darnstrom.github.io/daqp/parameters>`_ for a complete list of exitflags\n    info :\n        Contains additional information from the solver:\n           * setup_time : Time for settings up the problem\n           * solve_time : Time for solving the problem\n           * iterations : Number of performed iterations\n           * nodes      : Explored nodes in branch-and-bound tree\n           * lam        : Optimal dual solution\n    ";
+static PyMethodDef __pyx_mdef_4daqp_1solve = {"solve", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4daqp_1solve, METH_VARARGS|METH_KEYWORDS, __pyx_doc_4daqp_solve};
 static PyObject *__pyx_pw_4daqp_1solve(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_H = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_f = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_A = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bupper = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_blower = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sense = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -2605,19 +2619,24 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4daqp_solve(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_H, __Pyx_memviewslice __pyx_v_f, __Pyx_memviewslice __pyx_v_A, __Pyx_memviewslice __pyx_v_bupper, __Pyx_memviewslice __pyx_v_blower, __Pyx_memviewslice __pyx_v_sense, PyObject *__pyx_v_primal_tol, PyObject *__pyx_v_dual_tol, PyObject *__pyx_v_zero_tol, PyObject *__pyx_v_pivot_tol, PyObject *__pyx_v_progress_tol, PyObject *__pyx_v_cycle_tol, PyObject *__pyx_v_iter_limit, PyObject *__pyx_v_fval_bound, PyObject *__pyx_v_eps_prox, PyObject *__pyx_v_eta_prox, PyObject *__pyx_v_rho_soft, PyObject *__pyx_v_rel_subopt, PyObject *__pyx_v_abs_subopt) {
   int __pyx_v_n;
   int __pyx_v_m;
+  double *__pyx_v_A_ptr;
+  double *__pyx_v_bu_ptr;
+  double *__pyx_v_bl_ptr;
+  int *__pyx_v_sense_ptr;
   PyObject *__pyx_v_mA = NULL;
   DAQPProblem __pyx_v_problem;
   DAQPSettings __pyx_v_settings;
   __Pyx_memviewslice __pyx_v_x = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_lam = { 0, 0, { 0 }, { 0 }, { 0 } };
+  double *__pyx_v_lam_ptr;
   DAQPResult __pyx_v_res;
   PyObject *__pyx_v_info = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2626,221 +2645,222 @@
   PyObject *(*__pyx_t_6)(PyObject *);
   int __pyx_t_7;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   __Pyx_memviewslice __pyx_t_11 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_t_12 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  Py_ssize_t __pyx_t_13;
+  void *__pyx_t_13;
   Py_ssize_t __pyx_t_14;
-  int __pyx_t_15;
-  Py_ssize_t __pyx_t_16;
-  Py_ssize_t __pyx_t_17;
-  Py_ssize_t __pyx_t_18;
-  Py_ssize_t __pyx_t_19;
-  Py_ssize_t __pyx_t_20;
-  Py_ssize_t __pyx_t_21;
-  DAQPProblem __pyx_t_22;
-  double __pyx_t_23;
+  Py_ssize_t __pyx_t_15;
+  void *__pyx_t_16;
+  void *__pyx_t_17;
+  double *__pyx_t_18;
+  double *__pyx_t_19;
+  int *__pyx_t_20;
+  int __pyx_t_21;
+  Py_ssize_t __pyx_t_22;
+  DAQPProblem __pyx_t_23;
   double __pyx_t_24;
   double __pyx_t_25;
   double __pyx_t_26;
   double __pyx_t_27;
   double __pyx_t_28;
   double __pyx_t_29;
   double __pyx_t_30;
   double __pyx_t_31;
   double __pyx_t_32;
   double __pyx_t_33;
-  DAQPSettings __pyx_t_34;
-  __Pyx_memviewslice __pyx_t_35 = { 0, 0, { 0 }, { 0 }, { 0 } };
-  DAQPResult __pyx_t_36;
+  double __pyx_t_34;
+  DAQPSettings __pyx_t_35;
+  __Pyx_memviewslice __pyx_t_36 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  DAQPResult __pyx_t_37;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("solve", 0);
 
-  /* "daqp.pyx":14
- *     cdef int n,m,ms,nb
- *     cdef int* bin_ids_cand
+  /* "daqp.pyx":86
+ *     cdef double *A_ptr, *bu_ptr, *bl_ptr
+ *     cdef int* sense_ptr
  *     A = np.ascontiguousarray(A)             # <<<<<<<<<<<<<<
  *     mA, n = np.shape(A)
  *     m = np.size(bupper)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_ascontiguousarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 14, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 14, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_to_MemoryviewSlice_dsds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_5.memview)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_XDEC_MEMVIEW(&__pyx_v_A, 1);
   __pyx_v_A = __pyx_t_5;
   __pyx_t_5.memview = NULL;
   __pyx_t_5.data = NULL;
 
-  /* "daqp.pyx":15
- *     cdef int* bin_ids_cand
+  /* "daqp.pyx":87
+ *     cdef int* sense_ptr
  *     A = np.ascontiguousarray(A)
  *     mA, n = np.shape(A)             # <<<<<<<<<<<<<<
  *     m = np.size(bupper)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_shape); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_A, 2, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 15, __pyx_L1_error)
+      __PYX_ERR(0, 87, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 15, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_4), 2) < 0) __PYX_ERR(0, 87, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 15, __pyx_L1_error)
+    __PYX_ERR(0, 87, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_mA = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_n = __pyx_t_7;
 
-  /* "daqp.pyx":16
+  /* "daqp.pyx":88
  *     A = np.ascontiguousarray(A)
  *     mA, n = np.shape(A)
  *     m = np.size(bupper)             # <<<<<<<<<<<<<<
  * 
- *     if blower is None:
+ *     # By default, set lower bounds to -inf and interpret constraints as inequalities
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_bupper, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_bupper, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_m = __pyx_t_7;
 
-  /* "daqp.pyx":18
- *     m = np.size(bupper)
+  /* "daqp.pyx":91
  * 
+ *     # By default, set lower bounds to -inf and interpret constraints as inequalities
  *     if blower is None:             # <<<<<<<<<<<<<<
  *         blower = np.fill(m, -DAQP_INF)
  *     if sense is None:
  */
   __pyx_t_8 = ((((PyObject *) __pyx_v_blower.memview) == Py_None) != 0);
   if (__pyx_t_8) {
 
-    /* "daqp.pyx":19
- * 
+    /* "daqp.pyx":92
+ *     # By default, set lower bounds to -inf and interpret constraints as inequalities
  *     if blower is None:
  *         blower = np.fill(m, -DAQP_INF)             # <<<<<<<<<<<<<<
  *     if sense is None:
  *         sense = np.zeros(m, dtype=int)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fill); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_fill); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = PyFloat_FromDouble((-DAQP_INF)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble((-DAQP_INF)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_9 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_9)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -2849,561 +2869,626 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_9, __pyx_t_2, __pyx_t_4};
-      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else
     #endif
     {
-      __pyx_t_10 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       if (__pyx_t_9) {
         __Pyx_GIVEREF(__pyx_t_9); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_9); __pyx_t_9 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_2);
       PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_7, __pyx_t_2);
       __Pyx_GIVEREF(__pyx_t_4);
       PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_7, __pyx_t_4);
       __pyx_t_2 = 0;
       __pyx_t_4 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 19, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_to_MemoryviewSlice_ds_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_11.memview)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_XDEC_MEMVIEW(&__pyx_v_blower, 1);
     __pyx_v_blower = __pyx_t_11;
     __pyx_t_11.memview = NULL;
     __pyx_t_11.data = NULL;
 
-    /* "daqp.pyx":18
- *     m = np.size(bupper)
+    /* "daqp.pyx":91
  * 
+ *     # By default, set lower bounds to -inf and interpret constraints as inequalities
  *     if blower is None:             # <<<<<<<<<<<<<<
  *         blower = np.fill(m, -DAQP_INF)
  *     if sense is None:
  */
   }
 
-  /* "daqp.pyx":20
+  /* "daqp.pyx":93
  *     if blower is None:
  *         blower = np.fill(m, -DAQP_INF)
  *     if sense is None:             # <<<<<<<<<<<<<<
  *         sense = np.zeros(m, dtype=int)
  * 
  */
   __pyx_t_8 = ((((PyObject *) __pyx_v_sense.memview) == Py_None) != 0);
   if (__pyx_t_8) {
 
-    /* "daqp.pyx":21
+    /* "daqp.pyx":94
  *         blower = np.fill(m, -DAQP_INF)
  *     if sense is None:
  *         sense = np.zeros(m, dtype=int)             # <<<<<<<<<<<<<<
  * 
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
+ *     A_ptr = NULL if mA == 0 else &A[0,0]
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_10 = PyTuple_New(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
     __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyInt_Type))) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyInt_Type))) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 21, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyObject_to_MemoryviewSlice_ds_int(__pyx_t_4, PyBUF_WRITABLE); if (unlikely(!__pyx_t_12.memview)) __PYX_ERR(0, 94, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __PYX_XDEC_MEMVIEW(&__pyx_v_sense, 1);
     __pyx_v_sense = __pyx_t_12;
     __pyx_t_12.memview = NULL;
     __pyx_t_12.data = NULL;
 
-    /* "daqp.pyx":20
+    /* "daqp.pyx":93
  *     if blower is None:
  *         blower = np.fill(m, -DAQP_INF)
  *     if sense is None:             # <<<<<<<<<<<<<<
  *         sense = np.zeros(m, dtype=int)
  * 
  */
   }
 
-  /* "daqp.pyx":23
+  /* "daqp.pyx":96
  *         sense = np.zeros(m, dtype=int)
  * 
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],             # <<<<<<<<<<<<<<
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
+ *     A_ptr = NULL if mA == 0 else &A[0,0]             # <<<<<<<<<<<<<<
  * 
+ *     if m == 0:
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 23, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_EqObjC(__pyx_v_mA, __pyx_int_0, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyNumber_Subtract(__pyx_t_4, __pyx_v_mA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_13 = 0;
-  __pyx_t_14 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_13 < 0) {
-    __pyx_t_13 += __pyx_v_H.shape[0];
-    if (unlikely(__pyx_t_13 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_13 >= __pyx_v_H.shape[0])) __pyx_t_15 = 0;
-  if (__pyx_t_14 < 0) {
-    __pyx_t_14 += __pyx_v_H.shape[1];
-    if (unlikely(__pyx_t_14 < 0)) __pyx_t_15 = 1;
-  } else if (unlikely(__pyx_t_14 >= __pyx_v_H.shape[1])) __pyx_t_15 = 1;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 23, __pyx_L1_error)
-  }
-  __pyx_t_16 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_16 < 0) {
-    __pyx_t_16 += __pyx_v_f.shape[0];
-    if (unlikely(__pyx_t_16 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_16 >= __pyx_v_f.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 23, __pyx_L1_error)
+  if (__pyx_t_8) {
+    __pyx_t_13 = NULL;
+  } else {
+    __pyx_t_14 = 0;
+    __pyx_t_15 = 0;
+    __pyx_t_7 = -1;
+    if (__pyx_t_14 < 0) {
+      __pyx_t_14 += __pyx_v_A.shape[0];
+      if (unlikely(__pyx_t_14 < 0)) __pyx_t_7 = 0;
+    } else if (unlikely(__pyx_t_14 >= __pyx_v_A.shape[0])) __pyx_t_7 = 0;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_A.shape[1];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_7 = 1;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_A.shape[1])) __pyx_t_7 = 1;
+    if (unlikely(__pyx_t_7 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_7);
+      __PYX_ERR(0, 96, __pyx_L1_error)
+    }
+    __pyx_t_13 = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_A.data + __pyx_t_14 * __pyx_v_A.strides[0]) ) + __pyx_t_15 * __pyx_v_A.strides[1]) ))));
+  }
+  __pyx_v_A_ptr = __pyx_t_13;
+
+  /* "daqp.pyx":98
+ *     A_ptr = NULL if mA == 0 else &A[0,0]
+ * 
+ *     if m == 0:             # <<<<<<<<<<<<<<
+ *         bu_ptr, bl_ptr, sense_ptr = NULL, NULL, NULL
+ *     else:
+ */
+  __pyx_t_8 = ((__pyx_v_m == 0) != 0);
+  if (__pyx_t_8) {
+
+    /* "daqp.pyx":99
+ * 
+ *     if m == 0:
+ *         bu_ptr, bl_ptr, sense_ptr = NULL, NULL, NULL             # <<<<<<<<<<<<<<
+ *     else:
+ *         bu_ptr, bl_ptr, sense_ptr  = &bupper[0], &blower[0], &sense[0]
+ */
+    __pyx_t_13 = NULL;
+    __pyx_t_16 = NULL;
+    __pyx_t_17 = NULL;
+    __pyx_v_bu_ptr = __pyx_t_13;
+    __pyx_v_bl_ptr = __pyx_t_16;
+    __pyx_v_sense_ptr = __pyx_t_17;
+
+    /* "daqp.pyx":98
+ *     A_ptr = NULL if mA == 0 else &A[0,0]
+ * 
+ *     if m == 0:             # <<<<<<<<<<<<<<
+ *         bu_ptr, bl_ptr, sense_ptr = NULL, NULL, NULL
+ *     else:
+ */
+    goto __pyx_L7;
   }
 
-  /* "daqp.pyx":24
+  /* "daqp.pyx":101
+ *         bu_ptr, bl_ptr, sense_ptr = NULL, NULL, NULL
+ *     else:
+ *         bu_ptr, bl_ptr, sense_ptr  = &bupper[0], &blower[0], &sense[0]             # <<<<<<<<<<<<<<
  * 
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]             # <<<<<<<<<<<<<<
  * 
- *     # Setup settings
  */
-  __pyx_t_17 = 0;
-  __pyx_t_18 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_17 < 0) {
-    __pyx_t_17 += __pyx_v_A.shape[0];
-    if (unlikely(__pyx_t_17 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_17 >= __pyx_v_A.shape[0])) __pyx_t_15 = 0;
-  if (__pyx_t_18 < 0) {
-    __pyx_t_18 += __pyx_v_A.shape[1];
-    if (unlikely(__pyx_t_18 < 0)) __pyx_t_15 = 1;
-  } else if (unlikely(__pyx_t_18 >= __pyx_v_A.shape[1])) __pyx_t_15 = 1;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_t_19 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_19 < 0) {
-    __pyx_t_19 += __pyx_v_bupper.shape[0];
-    if (unlikely(__pyx_t_19 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_19 >= __pyx_v_bupper.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_t_20 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_20 < 0) {
-    __pyx_t_20 += __pyx_v_blower.shape[0];
-    if (unlikely(__pyx_t_20 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_20 >= __pyx_v_blower.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 24, __pyx_L1_error)
-  }
-  __pyx_t_21 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_21 < 0) {
-    __pyx_t_21 += __pyx_v_sense.shape[0];
-    if (unlikely(__pyx_t_21 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_21 >= __pyx_v_sense.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 24, __pyx_L1_error)
+  /*else*/ {
+    __pyx_t_15 = 0;
+    __pyx_t_7 = -1;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_bupper.shape[0];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_7 = 0;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_bupper.shape[0])) __pyx_t_7 = 0;
+    if (unlikely(__pyx_t_7 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_7);
+      __PYX_ERR(0, 101, __pyx_L1_error)
+    }
+    __pyx_t_18 = (&(*((double *) ( /* dim=0 */ (__pyx_v_bupper.data + __pyx_t_15 * __pyx_v_bupper.strides[0]) ))));
+    __pyx_t_15 = 0;
+    __pyx_t_7 = -1;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_blower.shape[0];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_7 = 0;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_blower.shape[0])) __pyx_t_7 = 0;
+    if (unlikely(__pyx_t_7 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_7);
+      __PYX_ERR(0, 101, __pyx_L1_error)
+    }
+    __pyx_t_19 = (&(*((double *) ( /* dim=0 */ (__pyx_v_blower.data + __pyx_t_15 * __pyx_v_blower.strides[0]) ))));
+    __pyx_t_15 = 0;
+    __pyx_t_7 = -1;
+    if (__pyx_t_15 < 0) {
+      __pyx_t_15 += __pyx_v_sense.shape[0];
+      if (unlikely(__pyx_t_15 < 0)) __pyx_t_7 = 0;
+    } else if (unlikely(__pyx_t_15 >= __pyx_v_sense.shape[0])) __pyx_t_7 = 0;
+    if (unlikely(__pyx_t_7 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_7);
+      __PYX_ERR(0, 101, __pyx_L1_error)
+    }
+    __pyx_t_20 = (&(*((int *) ( /* dim=0 */ (__pyx_v_sense.data + __pyx_t_15 * __pyx_v_sense.strides[0]) ))));
+    __pyx_v_bu_ptr = __pyx_t_18;
+    __pyx_v_bl_ptr = __pyx_t_19;
+    __pyx_v_sense_ptr = __pyx_t_20;
   }
+  __pyx_L7:;
 
-  /* "daqp.pyx":23
- *         sense = np.zeros(m, dtype=int)
+  /* "daqp.pyx":104
  * 
- *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0],             # <<<<<<<<<<<<<<
- *             &A[0,0], &bupper[0], &blower[0], &sense[0], NULL,0]
  * 
+ *     cdef DAQPProblem problem = [n,m,m-mA, &H[0,0], &f[0], A_ptr, bu_ptr, bl_ptr, sense_ptr]             # <<<<<<<<<<<<<<
+ * 
+ *     # Setup settings
  */
-  __pyx_t_22.n = __pyx_v_n;
-  __pyx_t_22.m = __pyx_v_m;
-  __pyx_t_22.ms = __pyx_t_7;
-  __pyx_t_22.H = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_H.data + __pyx_t_13 * __pyx_v_H.strides[0]) ) + __pyx_t_14 * __pyx_v_H.strides[1]) ))));
-  __pyx_t_22.f = (&(*((double *) ( /* dim=0 */ (__pyx_v_f.data + __pyx_t_16 * __pyx_v_f.strides[0]) ))));
-  __pyx_t_22.A = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_A.data + __pyx_t_17 * __pyx_v_A.strides[0]) ) + __pyx_t_18 * __pyx_v_A.strides[1]) ))));
-  __pyx_t_22.bupper = (&(*((double *) ( /* dim=0 */ (__pyx_v_bupper.data + __pyx_t_19 * __pyx_v_bupper.strides[0]) ))));
-  __pyx_t_22.blower = (&(*((double *) ( /* dim=0 */ (__pyx_v_blower.data + __pyx_t_20 * __pyx_v_blower.strides[0]) ))));
-  __pyx_t_22.sense = (&(*((int *) ( /* dim=0 */ (__pyx_v_sense.data + __pyx_t_21 * __pyx_v_sense.strides[0]) ))));
-  __pyx_t_22.bin_ids = NULL;
-  __pyx_t_22.nb = 0;
-  __pyx_v_problem = __pyx_t_22;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = PyNumber_Subtract(__pyx_t_4, __pyx_v_mA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_15 = 0;
+  __pyx_t_14 = 0;
+  __pyx_t_21 = -1;
+  if (__pyx_t_15 < 0) {
+    __pyx_t_15 += __pyx_v_H.shape[0];
+    if (unlikely(__pyx_t_15 < 0)) __pyx_t_21 = 0;
+  } else if (unlikely(__pyx_t_15 >= __pyx_v_H.shape[0])) __pyx_t_21 = 0;
+  if (__pyx_t_14 < 0) {
+    __pyx_t_14 += __pyx_v_H.shape[1];
+    if (unlikely(__pyx_t_14 < 0)) __pyx_t_21 = 1;
+  } else if (unlikely(__pyx_t_14 >= __pyx_v_H.shape[1])) __pyx_t_21 = 1;
+  if (unlikely(__pyx_t_21 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_21);
+    __PYX_ERR(0, 104, __pyx_L1_error)
+  }
+  __pyx_t_22 = 0;
+  __pyx_t_21 = -1;
+  if (__pyx_t_22 < 0) {
+    __pyx_t_22 += __pyx_v_f.shape[0];
+    if (unlikely(__pyx_t_22 < 0)) __pyx_t_21 = 0;
+  } else if (unlikely(__pyx_t_22 >= __pyx_v_f.shape[0])) __pyx_t_21 = 0;
+  if (unlikely(__pyx_t_21 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_21);
+    __PYX_ERR(0, 104, __pyx_L1_error)
+  }
+  __pyx_t_23.n = __pyx_v_n;
+  __pyx_t_23.m = __pyx_v_m;
+  __pyx_t_23.ms = __pyx_t_7;
+  __pyx_t_23.H = (&(*((double *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_H.data + __pyx_t_15 * __pyx_v_H.strides[0]) ) + __pyx_t_14 * __pyx_v_H.strides[1]) ))));
+  __pyx_t_23.f = (&(*((double *) ( /* dim=0 */ (__pyx_v_f.data + __pyx_t_22 * __pyx_v_f.strides[0]) ))));
+  __pyx_t_23.A = __pyx_v_A_ptr;
+  __pyx_t_23.bupper = __pyx_v_bu_ptr;
+  __pyx_t_23.blower = __pyx_v_bl_ptr;
+  __pyx_t_23.sense = __pyx_v_sense_ptr;
+  __pyx_v_problem = __pyx_t_23;
 
-  /* "daqp.pyx":27
+  /* "daqp.pyx":107
  * 
  *     # Setup settings
  *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,             # <<<<<<<<<<<<<<
  *             progress_tol, cycle_tol, iter_limit, fval_bound,
  *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
  */
-  __pyx_t_23 = __pyx_PyFloat_AsDouble(__pyx_v_primal_tol); if (unlikely((__pyx_t_23 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
-  __pyx_t_24 = __pyx_PyFloat_AsDouble(__pyx_v_dual_tol); if (unlikely((__pyx_t_24 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
-  __pyx_t_25 = __pyx_PyFloat_AsDouble(__pyx_v_zero_tol); if (unlikely((__pyx_t_25 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
-  __pyx_t_26 = __pyx_PyFloat_AsDouble(__pyx_v_pivot_tol); if (unlikely((__pyx_t_26 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_24 = __pyx_PyFloat_AsDouble(__pyx_v_primal_tol); if (unlikely((__pyx_t_24 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_25 = __pyx_PyFloat_AsDouble(__pyx_v_dual_tol); if (unlikely((__pyx_t_25 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_26 = __pyx_PyFloat_AsDouble(__pyx_v_zero_tol); if (unlikely((__pyx_t_26 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_27 = __pyx_PyFloat_AsDouble(__pyx_v_pivot_tol); if (unlikely((__pyx_t_27 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L1_error)
 
-  /* "daqp.pyx":28
+  /* "daqp.pyx":108
  *     # Setup settings
  *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,
  *             progress_tol, cycle_tol, iter_limit, fval_bound,             # <<<<<<<<<<<<<<
  *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
  * 
  */
-  __pyx_t_27 = __pyx_PyFloat_AsDouble(__pyx_v_progress_tol); if (unlikely((__pyx_t_27 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_cycle_tol); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_15 = __Pyx_PyInt_As_int(__pyx_v_iter_limit); if (unlikely((__pyx_t_15 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_t_28 = __pyx_PyFloat_AsDouble(__pyx_v_fval_bound); if (unlikely((__pyx_t_28 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 28, __pyx_L1_error)
+  __pyx_t_28 = __pyx_PyFloat_AsDouble(__pyx_v_progress_tol); if (unlikely((__pyx_t_28 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_v_cycle_tol); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_21 = __Pyx_PyInt_As_int(__pyx_v_iter_limit); if (unlikely((__pyx_t_21 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_v_fval_bound); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
 
-  /* "daqp.pyx":29
+  /* "daqp.pyx":109
  *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,
  *             progress_tol, cycle_tol, iter_limit, fval_bound,
  *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]             # <<<<<<<<<<<<<<
  * 
  *     # Setup output
  */
-  __pyx_t_29 = __pyx_PyFloat_AsDouble(__pyx_v_eps_prox); if (unlikely((__pyx_t_29 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_t_30 = __pyx_PyFloat_AsDouble(__pyx_v_eta_prox); if (unlikely((__pyx_t_30 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_t_31 = __pyx_PyFloat_AsDouble(__pyx_v_rho_soft); if (unlikely((__pyx_t_31 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_t_32 = __pyx_PyFloat_AsDouble(__pyx_v_rel_subopt); if (unlikely((__pyx_t_32 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
-  __pyx_t_33 = __pyx_PyFloat_AsDouble(__pyx_v_abs_subopt); if (unlikely((__pyx_t_33 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_30 = __pyx_PyFloat_AsDouble(__pyx_v_eps_prox); if (unlikely((__pyx_t_30 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_31 = __pyx_PyFloat_AsDouble(__pyx_v_eta_prox); if (unlikely((__pyx_t_31 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_32 = __pyx_PyFloat_AsDouble(__pyx_v_rho_soft); if (unlikely((__pyx_t_32 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_33 = __pyx_PyFloat_AsDouble(__pyx_v_rel_subopt); if (unlikely((__pyx_t_33 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_34 = __pyx_PyFloat_AsDouble(__pyx_v_abs_subopt); if (unlikely((__pyx_t_34 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
 
-  /* "daqp.pyx":27
+  /* "daqp.pyx":107
  * 
  *     # Setup settings
  *     cdef DAQPSettings settings = [primal_tol, dual_tol, zero_tol, pivot_tol,             # <<<<<<<<<<<<<<
  *             progress_tol, cycle_tol, iter_limit, fval_bound,
  *             eps_prox, eta_prox, rho_soft, rel_subopt, abs_subopt]
  */
-  __pyx_t_34.primal_tol = __pyx_t_23;
-  __pyx_t_34.dual_tol = __pyx_t_24;
-  __pyx_t_34.zero_tol = __pyx_t_25;
-  __pyx_t_34.pivot_tol = __pyx_t_26;
-  __pyx_t_34.progress_tol = __pyx_t_27;
-  __pyx_t_34.cycle_tol = __pyx_t_7;
-  __pyx_t_34.iter_limit = __pyx_t_15;
-  __pyx_t_34.fval_bound = __pyx_t_28;
-  __pyx_t_34.eps_prox = __pyx_t_29;
-  __pyx_t_34.eta_prox = __pyx_t_30;
-  __pyx_t_34.rho_soft = __pyx_t_31;
-  __pyx_t_34.rel_subopt = __pyx_t_32;
-  __pyx_t_34.abs_subopt = __pyx_t_33;
-  __pyx_v_settings = __pyx_t_34;
+  __pyx_t_35.primal_tol = __pyx_t_24;
+  __pyx_t_35.dual_tol = __pyx_t_25;
+  __pyx_t_35.zero_tol = __pyx_t_26;
+  __pyx_t_35.pivot_tol = __pyx_t_27;
+  __pyx_t_35.progress_tol = __pyx_t_28;
+  __pyx_t_35.cycle_tol = __pyx_t_7;
+  __pyx_t_35.iter_limit = __pyx_t_21;
+  __pyx_t_35.fval_bound = __pyx_t_29;
+  __pyx_t_35.eps_prox = __pyx_t_30;
+  __pyx_t_35.eta_prox = __pyx_t_31;
+  __pyx_t_35.rho_soft = __pyx_t_32;
+  __pyx_t_35.rel_subopt = __pyx_t_33;
+  __pyx_t_35.abs_subopt = __pyx_t_34;
+  __pyx_v_settings = __pyx_t_35;
 
-  /* "daqp.pyx":32
+  /* "daqp.pyx":112
  * 
  *     # Setup output
  *     cdef double[::1] x = np.zeros(n)             # <<<<<<<<<<<<<<
  *     cdef double[::1] lam = np.zeros(m)
- *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
+ *     cdef double *lam_ptr
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_10))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_10);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_10, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_10, __pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_10, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __pyx_t_36 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_36.memview)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_x = __pyx_t_35;
-  __pyx_t_35.memview = NULL;
-  __pyx_t_35.data = NULL;
+  __pyx_v_x = __pyx_t_36;
+  __pyx_t_36.memview = NULL;
+  __pyx_t_36.data = NULL;
 
-  /* "daqp.pyx":33
+  /* "daqp.pyx":113
  *     # Setup output
  *     cdef double[::1] x = np.zeros(n)
  *     cdef double[::1] lam = np.zeros(m)             # <<<<<<<<<<<<<<
- *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]
- * 
+ *     cdef double *lam_ptr
+ *     lam_ptr = NULL if m == 0 else &lam[0]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_m); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_10);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_35 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_35.memview)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_36 = __Pyx_PyObject_to_MemoryviewSlice_dc_double(__pyx_t_1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_36.memview)) __PYX_ERR(0, 113, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v_lam = __pyx_t_35;
-  __pyx_t_35.memview = NULL;
-  __pyx_t_35.data = NULL;
+  __pyx_v_lam = __pyx_t_36;
+  __pyx_t_36.memview = NULL;
+  __pyx_t_36.data = NULL;
 
-  /* "daqp.pyx":34
- *     cdef double[::1] x = np.zeros(n)
+  /* "daqp.pyx":115
  *     cdef double[::1] lam = np.zeros(m)
- *     cdef DAQPResult res  = [&x[0],&lam[0],0,0,0,0,0,0,0]             # <<<<<<<<<<<<<<
+ *     cdef double *lam_ptr
+ *     lam_ptr = NULL if m == 0 else &lam[0]             # <<<<<<<<<<<<<<
+ *     cdef DAQPResult res  = [&x[0],lam_ptr,0,0,0,0,0,0,0]
+ * 
+ */
+  if (((__pyx_v_m == 0) != 0)) {
+    __pyx_t_17 = NULL;
+  } else {
+    __pyx_t_22 = 0;
+    __pyx_t_21 = -1;
+    if (__pyx_t_22 < 0) {
+      __pyx_t_22 += __pyx_v_lam.shape[0];
+      if (unlikely(__pyx_t_22 < 0)) __pyx_t_21 = 0;
+    } else if (unlikely(__pyx_t_22 >= __pyx_v_lam.shape[0])) __pyx_t_21 = 0;
+    if (unlikely(__pyx_t_21 != -1)) {
+      __Pyx_RaiseBufferIndexError(__pyx_t_21);
+      __PYX_ERR(0, 115, __pyx_L1_error)
+    }
+    __pyx_t_17 = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_22)) ))));
+  }
+  __pyx_v_lam_ptr = __pyx_t_17;
+
+  /* "daqp.pyx":116
+ *     cdef double *lam_ptr
+ *     lam_ptr = NULL if m == 0 else &lam[0]
+ *     cdef DAQPResult res  = [&x[0],lam_ptr,0,0,0,0,0,0,0]             # <<<<<<<<<<<<<<
  * 
  *     # Solve
  */
-  __pyx_t_21 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_21 < 0) {
-    __pyx_t_21 += __pyx_v_x.shape[0];
-    if (unlikely(__pyx_t_21 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_21 >= __pyx_v_x.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 34, __pyx_L1_error)
-  }
-  __pyx_t_20 = 0;
-  __pyx_t_15 = -1;
-  if (__pyx_t_20 < 0) {
-    __pyx_t_20 += __pyx_v_lam.shape[0];
-    if (unlikely(__pyx_t_20 < 0)) __pyx_t_15 = 0;
-  } else if (unlikely(__pyx_t_20 >= __pyx_v_lam.shape[0])) __pyx_t_15 = 0;
-  if (unlikely(__pyx_t_15 != -1)) {
-    __Pyx_RaiseBufferIndexError(__pyx_t_15);
-    __PYX_ERR(0, 34, __pyx_L1_error)
-  }
-  __pyx_t_36.x = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_x.data) + __pyx_t_21)) ))));
-  __pyx_t_36.lam = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_lam.data) + __pyx_t_20)) ))));
-  __pyx_t_36.fval = 0.0;
-  __pyx_t_36.soft_slack = 0.0;
-  __pyx_t_36.exitflag = 0;
-  __pyx_t_36.iter = 0;
-  __pyx_t_36.nodes = 0;
-  __pyx_t_36.solve_time = 0.0;
-  __pyx_t_36.setup_time = 0.0;
-  __pyx_v_res = __pyx_t_36;
+  __pyx_t_22 = 0;
+  __pyx_t_21 = -1;
+  if (__pyx_t_22 < 0) {
+    __pyx_t_22 += __pyx_v_x.shape[0];
+    if (unlikely(__pyx_t_22 < 0)) __pyx_t_21 = 0;
+  } else if (unlikely(__pyx_t_22 >= __pyx_v_x.shape[0])) __pyx_t_21 = 0;
+  if (unlikely(__pyx_t_21 != -1)) {
+    __Pyx_RaiseBufferIndexError(__pyx_t_21);
+    __PYX_ERR(0, 116, __pyx_L1_error)
+  }
+  __pyx_t_37.x = (&(*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_x.data) + __pyx_t_22)) ))));
+  __pyx_t_37.lam = __pyx_v_lam_ptr;
+  __pyx_t_37.fval = 0.0;
+  __pyx_t_37.soft_slack = 0.0;
+  __pyx_t_37.exitflag = 0;
+  __pyx_t_37.iter = 0;
+  __pyx_t_37.nodes = 0;
+  __pyx_t_37.solve_time = 0.0;
+  __pyx_t_37.setup_time = 0.0;
+  __pyx_v_res = __pyx_t_37;
 
-  /* "daqp.pyx":37
+  /* "daqp.pyx":119
  * 
  *     # Solve
  *     with nogil:             # <<<<<<<<<<<<<<
  *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "daqp.pyx":38
+        /* "daqp.pyx":120
  *     # Solve
  *     with nogil:
  *         daqp_quadprog(&res, &problem, &settings)             # <<<<<<<<<<<<<<
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,
  */
         (void)(daqp_quadprog((&__pyx_v_res), (&__pyx_v_problem), (&__pyx_v_settings)));
       }
 
-      /* "daqp.pyx":37
+      /* "daqp.pyx":119
  * 
  *     # Solve
  *     with nogil:             # <<<<<<<<<<<<<<
  *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
-          goto __pyx_L9;
+          goto __pyx_L10;
         }
-        __pyx_L9:;
+        __pyx_L10:;
       }
   }
 
-  /* "daqp.pyx":39
+  /* "daqp.pyx":121
  *     with nogil:
  *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,             # <<<<<<<<<<<<<<
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.solve_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.solve_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_solve_time, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_solve_time, __pyx_t_4) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":40
+  /* "daqp.pyx":122
  *         daqp_quadprog(&res, &problem, &settings)
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,             # <<<<<<<<<<<<<<
  *             'iterations': res.iter,
  *             'nodes': res.nodes,
  */
-  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.setup_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble(__pyx_v_res.setup_time); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_setup_time, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_setup_time, __pyx_t_4) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":41
+  /* "daqp.pyx":123
  *     info = {'solve_time':res.solve_time,
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,             # <<<<<<<<<<<<<<
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.iter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.iter); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_iterations, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_iterations, __pyx_t_4) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":42
+  /* "daqp.pyx":124
  *             'setup_time': res.setup_time,
  *             'iterations': res.iter,
  *             'nodes': res.nodes,             # <<<<<<<<<<<<<<
  *             'lam': np.asarray(lam)}
  *     return np.asarray(x), res.fval, res.exitflag, info
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.nodes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.nodes); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_nodes, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_nodes, __pyx_t_4) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "daqp.pyx":43
+  /* "daqp.pyx":125
  *             'iterations': res.iter,
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}             # <<<<<<<<<<<<<<
  *     return np.asarray(x), res.fval, res.exitflag, info
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_10, __pyx_n_s_np); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_10, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_lam, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_10 = __pyx_memoryview_fromslice(__pyx_v_lam, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_10) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_10);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_lam, __pyx_t_4) < 0) __PYX_ERR(0, 39, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_lam, __pyx_t_4) < 0) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_v_info = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "daqp.pyx":44
+  /* "daqp.pyx":126
  *             'nodes': res.nodes,
  *             'lam': np.asarray(lam)}
  *     return np.asarray(x), res.fval, res.exitflag, info             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_asarray); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_x, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_4 = __pyx_memoryview_fromslice(__pyx_v_x, 1, (PyObject *(*)(char *)) __pyx_memview_get_double, (int (*)(char *, PyObject *)) __pyx_memview_set_double, 0);; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_10 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_10)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_10);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_10, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_res.fval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_res.fval); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.exitflag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_res.exitflag); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_10 = PyTuple_New(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 44, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_t_4);
@@ -3432,15 +3517,15 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __PYX_XDEC_MEMVIEW(&__pyx_t_5, 1);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __PYX_XDEC_MEMVIEW(&__pyx_t_11, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_t_12, 1);
-  __PYX_XDEC_MEMVIEW(&__pyx_t_35, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_36, 1);
   __Pyx_AddTraceback("daqp.solve", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_mA);
   __PYX_XDEC_MEMVIEW(&__pyx_v_x, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_lam, 1);
   __Pyx_XDECREF(__pyx_v_info);
@@ -17267,14 +17352,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_n_s_A, __pyx_k_A, sizeof(__pyx_k_A), 0, 0, 1, 1},
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
+  {&__pyx_n_s_A_ptr, __pyx_k_A_ptr, sizeof(__pyx_k_A_ptr), 0, 0, 1, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
@@ -17296,15 +17382,17 @@
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_abs_subopt, __pyx_k_abs_subopt, sizeof(__pyx_k_abs_subopt), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_asarray, __pyx_k_asarray, sizeof(__pyx_k_asarray), 0, 0, 1, 1},
   {&__pyx_n_s_ascontiguousarray, __pyx_k_ascontiguousarray, sizeof(__pyx_k_ascontiguousarray), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_bin_ids_cand, __pyx_k_bin_ids_cand, sizeof(__pyx_k_bin_ids_cand), 0, 0, 1, 1},
+  {&__pyx_n_s_bl_ptr, __pyx_k_bl_ptr, sizeof(__pyx_k_bl_ptr), 0, 0, 1, 1},
   {&__pyx_n_s_blower, __pyx_k_blower, sizeof(__pyx_k_blower), 0, 0, 1, 1},
+  {&__pyx_n_s_bu_ptr, __pyx_k_bu_ptr, sizeof(__pyx_k_bu_ptr), 0, 0, 1, 1},
   {&__pyx_n_s_bupper, __pyx_k_bupper, sizeof(__pyx_k_bupper), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
   {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
   {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
@@ -17333,14 +17421,15 @@
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_info, __pyx_k_info, sizeof(__pyx_k_info), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_iter_limit, __pyx_k_iter_limit, sizeof(__pyx_k_iter_limit), 0, 0, 1, 1},
   {&__pyx_n_s_iterations, __pyx_k_iterations, sizeof(__pyx_k_iterations), 0, 0, 1, 1},
   {&__pyx_n_s_lam, __pyx_k_lam, sizeof(__pyx_k_lam), 0, 0, 1, 1},
+  {&__pyx_n_s_lam_ptr, __pyx_k_lam_ptr, sizeof(__pyx_k_lam_ptr), 0, 0, 1, 1},
   {&__pyx_n_s_m, __pyx_k_m, sizeof(__pyx_k_m), 0, 0, 1, 1},
   {&__pyx_n_s_mA, __pyx_k_mA, sizeof(__pyx_k_mA), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_ms, __pyx_k_ms, sizeof(__pyx_k_ms), 0, 0, 1, 1},
   {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
@@ -17372,14 +17461,15 @@
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_rel_subopt, __pyx_k_rel_subopt, sizeof(__pyx_k_rel_subopt), 0, 0, 1, 1},
   {&__pyx_n_s_res, __pyx_k_res, sizeof(__pyx_k_res), 0, 0, 1, 1},
   {&__pyx_n_s_rho_soft, __pyx_k_rho_soft, sizeof(__pyx_k_rho_soft), 0, 0, 1, 1},
   {&__pyx_n_s_sense, __pyx_k_sense, sizeof(__pyx_k_sense), 0, 0, 1, 1},
+  {&__pyx_n_s_sense_ptr, __pyx_k_sense_ptr, sizeof(__pyx_k_sense_ptr), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_settings, __pyx_k_settings, sizeof(__pyx_k_settings), 0, 0, 1, 1},
   {&__pyx_n_s_setup_time, __pyx_k_setup_time, sizeof(__pyx_k_setup_time), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_solve, __pyx_k_solve, sizeof(__pyx_k_solve), 0, 0, 1, 1},
@@ -17618,18 +17708,18 @@
   /* "daqp.pyx":4
  * cimport daqp
  * 
  * def solve(double[:, :] H, double[:] f, double[:, :] A,             # <<<<<<<<<<<<<<
  *         double[:] bupper, double[:] blower=None, int[:] sense =None,
  *         primal_tol = DEFAULT_PRIM_TOL, dual_tol = DEFAULT_DUAL_TOL, zero_tol = DEFAULT_ZERO_TOL,
  */
-  __pyx_tuple__34 = PyTuple_Pack(31, __pyx_n_s_H, __pyx_n_s_f, __pyx_n_s_A, __pyx_n_s_bupper, __pyx_n_s_blower, __pyx_n_s_sense, __pyx_n_s_primal_tol, __pyx_n_s_dual_tol, __pyx_n_s_zero_tol, __pyx_n_s_pivot_tol, __pyx_n_s_progress_tol, __pyx_n_s_cycle_tol, __pyx_n_s_iter_limit, __pyx_n_s_fval_bound, __pyx_n_s_eps_prox, __pyx_n_s_eta_prox, __pyx_n_s_rho_soft, __pyx_n_s_rel_subopt, __pyx_n_s_abs_subopt, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_ms, __pyx_n_s_nb, __pyx_n_s_bin_ids_cand, __pyx_n_s_mA, __pyx_n_s_problem, __pyx_n_s_settings, __pyx_n_s_x, __pyx_n_s_lam, __pyx_n_s_res, __pyx_n_s_info); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_tuple__34 = PyTuple_Pack(36, __pyx_n_s_H, __pyx_n_s_f, __pyx_n_s_A, __pyx_n_s_bupper, __pyx_n_s_blower, __pyx_n_s_sense, __pyx_n_s_primal_tol, __pyx_n_s_dual_tol, __pyx_n_s_zero_tol, __pyx_n_s_pivot_tol, __pyx_n_s_progress_tol, __pyx_n_s_cycle_tol, __pyx_n_s_iter_limit, __pyx_n_s_fval_bound, __pyx_n_s_eps_prox, __pyx_n_s_eta_prox, __pyx_n_s_rho_soft, __pyx_n_s_rel_subopt, __pyx_n_s_abs_subopt, __pyx_n_s_n, __pyx_n_s_m, __pyx_n_s_ms, __pyx_n_s_nb, __pyx_n_s_bin_ids_cand, __pyx_n_s_A_ptr, __pyx_n_s_bu_ptr, __pyx_n_s_bl_ptr, __pyx_n_s_sense_ptr, __pyx_n_s_mA, __pyx_n_s_problem, __pyx_n_s_settings, __pyx_n_s_x, __pyx_n_s_lam, __pyx_n_s_lam_ptr, __pyx_n_s_res, __pyx_n_s_info); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(19, 0, 31, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_daqp_pyx, __pyx_n_s_solve, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(19, 0, 36, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_daqp_pyx, __pyx_n_s_solve, 4, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 4, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
@@ -18131,15 +18221,15 @@
   __pyx_t_1 = 0;
 
   /* "daqp.pyx":9
  *         pivot_tol = DEFAULT_PIVOT_TOL, progress_tol = DEFAULT_PROG_TOL,
  *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
  *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,             # <<<<<<<<<<<<<<
  *         rel_subopt = DEFAULT_REL_SUBOPT, abs_subopt = DEFAULT_ABS_SUBOPT):
- *     # Setup problem
+ *     """
  */
   __pyx_t_1 = PyFloat_FromDouble(DEFAULT_ETA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_k__9 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_1 = PyFloat_FromDouble(DEFAULT_RHO_SOFT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
@@ -18148,16 +18238,16 @@
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "daqp.pyx":10
  *         cycle_tol = DEFAULT_CYCLE_TOL, iter_limit =  DEFAULT_ITER_LIMIT, fval_bound = DAQP_INF,
  *         eps_prox= 0, eta_prox = DEFAULT_ETA, rho_soft = DEFAULT_RHO_SOFT,
  *         rel_subopt = DEFAULT_REL_SUBOPT, abs_subopt = DEFAULT_ABS_SUBOPT):             # <<<<<<<<<<<<<<
- *     # Setup problem
- *     cdef int n,m,ms,nb
+ *     """
+ *     Solve the quadratic program      minimize       0.5 x'*H*x + f' x
  */
   __pyx_t_1 = PyFloat_FromDouble(DEFAULT_REL_SUBOPT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_k__11 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
   __pyx_t_1 = PyFloat_FromDouble(DEFAULT_ABS_SUBOPT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
@@ -19053,14 +19143,81 @@
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
     }
     return __Pyx_IterFinish();
 }
 
+/* PyIntCompare */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_EqObjC(PyObject *op1, PyObject *op2, CYTHON_UNUSED long intval, CYTHON_UNUSED long inplace) {
+    if (op1 == op2) {
+        Py_RETURN_TRUE;
+    }
+    #if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_CheckExact(op1))) {
+        const long b = intval;
+        long a = PyInt_AS_LONG(op1);
+        if (a == b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    #if CYTHON_USE_PYLONG_INTERNALS
+    if (likely(PyLong_CheckExact(op1))) {
+        int unequal;
+        unsigned long uintval;
+        Py_ssize_t size = Py_SIZE(op1);
+        const digit* digits = ((PyLongObject*)op1)->ob_digit;
+        if (intval == 0) {
+            if (size == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+        } else if (intval < 0) {
+            if (size >= 0)
+                Py_RETURN_FALSE;
+            intval = -intval;
+            size = -size;
+        } else {
+            if (size <= 0)
+                Py_RETURN_FALSE;
+        }
+        uintval = (unsigned long) intval;
+#if PyLong_SHIFT * 4 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 4)) {
+            unequal = (size != 5) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[4] != ((uintval >> (4 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 3 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 3)) {
+            unequal = (size != 4) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[3] != ((uintval >> (3 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 2 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 2)) {
+            unequal = (size != 3) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK)) | (digits[2] != ((uintval >> (2 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+#if PyLong_SHIFT * 1 < SIZEOF_LONG*8
+        if (uintval >> (PyLong_SHIFT * 1)) {
+            unequal = (size != 2) || (digits[0] != (uintval & (unsigned long) PyLong_MASK))
+                 | (digits[1] != ((uintval >> (1 * PyLong_SHIFT)) & (unsigned long) PyLong_MASK));
+        } else
+#endif
+            unequal = (size != 1) || (((unsigned long) digits[0]) != (uintval & (unsigned long) PyLong_MASK));
+        if (unequal == 0) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    #endif
+    if (PyFloat_CheckExact(op1)) {
+        const long b = intval;
+        double a = PyFloat_AS_DOUBLE(op1);
+        if ((double)a == (double)b) Py_RETURN_TRUE; else Py_RETURN_FALSE;
+    }
+    return (
+        PyObject_RichCompare(op1, op2, Py_EQ));
+}
+
 /* BufferIndexError */
 static void __Pyx_RaiseBufferIndexError(int axis) {
   PyErr_Format(PyExc_IndexError,
      "Out of bounds on buffer access (axis %d)", axis);
 }
 
 /* ArgTypeTest */
```

### Comparing `daqp-0.4.1/daqp.egg-info/PKG-INFO` & `daqp-0.5.0/daqp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daqp
-Version: 0.4.1
+Version: 0.5.0
 Summary: DAQP: A dual active-set QP solver
 Home-page: http://github.com/darnstrom/daqp
 Author: Daniel Arnström
 Author-email: daniel.arnstrom@liu.se
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daqp-0.4.1/daqp.egg-info/SOURCES.txt` & `daqp-0.5.0/daqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daqp-0.4.1/daqp.pxd` & `daqp-0.5.0/daqp.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,14 @@
     
         double* A
         double* bupper
         double* blower 
     
         int* sense
     
-        int* bin_ids
-        int nb
-    
     ctypedef struct DAQPSettings:
         double primal_tol;
         double dual_tol;
         double zero_tol;
         double pivot_tol;
         double progress_tol;
```

### Comparing `daqp-0.4.1/setup.py` & `daqp-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             'csrc/src/utils.c', 
             ],
         library_dirs=['.'],
         extra_compile_args=["-O3", "-DPROFILING"],
         include_dirs=['csrc/include'])
 
 setup(name='daqp',
-        version='0.4.1',
+        version='0.5.0',
         description='DAQP: A dual active-set QP solver',
         url='http://github.com/darnstrom/daqp',
         author='Daniel Arnström',
         author_email='daniel.arnstrom@liu.se',
         license='MIT',
         long_description=open('README.md','r').read(),
         long_description_content_type='text/markdown',
```

