# Comparing `tmp/bayanpy-0.5.tar.gz` & `tmp/bayanpy-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayanpy-0.5.tar", last modified: Sat Apr  8 16:18:10 2023, max compression
+gzip compressed data, was "bayanpy-0.6.tar", last modified: Tue Apr 11 16:04:35 2023, max compression
```

## Comparing `bayanpy-0.5.tar` & `bayanpy-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.5/LICENSE
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 16:18:10.947248 bayanpy-0.5/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     5077 2023-04-08 16:17:15.000000 bayanpy-0.5/README.md
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/bayanpy/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-08 16:13:17.000000 bayanpy-0.5/bayanpy/__init__.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    52003 2023-04-08 16:14:58.000000 bayanpy-0.5/bayanpy/bayanimplied.py
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    44347 2023-04-08 03:05:45.000000 bayanpy-0.5/bayanpy/bayanpy.py
-drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-08 16:18:10.947248 bayanpy-0.5/bayanpy.egg-info/
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/PKG-INFO
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      243 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/SOURCES.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/dependency_links.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/requires.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-08 16:18:10.000000 bayanpy-0.5/bayanpy.egg-info/top_level.txt
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-08 16:18:10.947248 bayanpy-0.5/setup.cfg
--rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      559 2023-04-08 16:17:39.000000 bayanpy-0.5/setup.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    18092 2022-10-14 23:15:16.000000 bayanpy-0.6/LICENSE
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-11 16:04:35.713202 bayanpy-0.6/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)     4917 2023-04-11 15:57:56.000000 bayanpy-0.6/README.md
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/bayanpy/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       62 2023-04-08 16:13:17.000000 bayanpy-0.6/bayanpy/__init__.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    51005 2023-04-11 16:03:12.000000 bayanpy-0.6/bayanpy/bayanImplied.py
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)    44347 2023-04-08 03:05:45.000000 bayanpy-0.6/bayanpy/bayanpy.py
+drwxrwxr-x   0 mahdi     (1000) mahdi     (1000)        0 2023-04-11 16:04:35.713202 bayanpy-0.6/bayanpy.egg-info/
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      357 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/PKG-INFO
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      243 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        1 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       53 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/requires.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)        8 2023-04-11 16:04:35.000000 bayanpy-0.6/bayanpy.egg-info/top_level.txt
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)       38 2023-04-11 16:04:35.713202 bayanpy-0.6/setup.cfg
+-rw-rw-r--   0 mahdi     (1000) mahdi     (1000)      559 2023-04-11 16:04:27.000000 bayanpy-0.6/setup.py
```

### Comparing `bayanpy-0.5/LICENSE` & `bayanpy-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bayanpy-0.5/README.md` & `bayanpy-0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,49 +53,47 @@
 
 5. Request an academic license from [the Gurobi academic license page](https://www.gurobi.com/downloads/end-user-license-agreement-academic/) and install the license on your computer following the instructions given on the Gurobi license page.
 
 For detailed installation instructions, refer to the Gurobi Quick Start Guides for [Windows](https://www.gurobi.com/documentation/9.5/quickstart_windows/index.html), [Linux](https://www.gurobi.com/documentation/9.5/quickstart_linux/index.html), or [macOS](https://www.gurobi.com/documentation/9.5/quickstart_mac/index.html).
 
 ## Usage
 
-You can use Bayanpy in two ways:
-
-### 1. As a standalone package (Recommended)
-
-After installing Bayanpy, you can use it directly in your Python code as follows:
+You can use Bayanpy as a standalone package. After installing Bayanpy, you can use it directly in your Python code as follows:
 
 ```python
 import networkx as nx
 import bayanpy
 
 # Create or load your networkx graph (undirected)
 graph = G = nx.karate_club_graph()
 
 # Run the Bayan algorithm
 modularity, optimality_gap, community = bayanpy.bayan(graph, threshold=0.001, time_allowed=60, resolution=1)
 ```
 
 
-### 2. Through the CDlib (Community Discovery library)
-
-Bayanpy can be used as part of the [CDlib](https://cdlib.readthedocs.io/en/latest/reference/cd_algorithms/algs/cdlib.algorithms.bayan.html) package. Follow the CDlib documentation for more details on how to use Bayan with CDlib.
 
 #### Parameters and acceptable input
 
 - `graph`: Input graph should be an undirected networkx graph. You can use the edge attribute "weight" to represent positive edge weights.
 - `threshold`: The acceptable optimality gap for the algorithm to terminate. If Bayan finds a solution with a modularity value within the specified threshold of the optimal solution, it stops the search and returns the found solution. For example, setting the threshold to 0.001 means Bayan will stop when it finds a solution within 0.1% of the optimal modularity value.
 - `time_allowed`: The maximum allowed execution time in seconds for Bayan to search for a solution. Once this time limit is reached, the algorithm will terminate and return the best solution found so far, even if the optimality gap threshold has not been met.
 - `resolution`: The resolution parameter in the modularity function.
 
 #### Returns
 
 - `modularity`: The modularity value of the returned partition.
 - `optimality_gap`: The guaranteed upper bound of the percentage difference between the modularity of the returned partition and the maximum modularity.
 - `community`: A nested list describing the community assignment of the returned partition.
 
+
+### Example
+You can find a few examples of different ways Bayan can be used at this Google Colab address: [bayanpy Examples](https://tinyurl.com/bayancolab)
+
+
 ## Contributing
 
 We welcome contributions to the Bayanpy project. If you have any suggestions or encounter any issues, please feel free to open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 Bayanpy is released under the [GNU General Public License](LICENSE). For more information, please refer to the [LICENSE](LICENSE) file in the repository.
```

### Comparing `bayanpy-0.5/bayanpy/bayanimplied.py` & `bayanpy-0.6/bayanpy/bayanImplied.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from gurobipy import *
 from cdlib import algorithms
 from networkx.algorithms.connectivity import minimum_st_node_cut
 from joblib import Parallel, delayed, parallel_backend
 from itertools import chain
 
 
-#Load Graph from network name
+# Load Graph from network name
 def get_graph_from_network_name(network_name, sub_name=None):
     """
     Method to create a networkx Graph from network names listed at https://networks.skewed.de/
     """
     #Defining the network information url
     info_url = "https://networks.skewed.de/api/net/%s" % network_name
     req = requests.get(info_url)
@@ -114,19 +114,14 @@
     
     # If G is a multigraph then the edge attributes correspond to the attributes of the last seen edge as in the data
     if is_multigraph:
         print("%s is a multigraph but has been loaded as a simple graph" % network_name)
     
     shutil.rmtree(network_name + "_files")
     return G
-
-
-# In[4]:
-
-
 def get_local_clustering_coefficient(G, node: int):
     """
     Returns the clustering coefficient for the input node in the input graph
     """
     neighbours = nx.adjacency_matrix(G)[node].indices
     if neighbours.shape[0] <= 1:
         return 0.0
@@ -194,24 +189,20 @@
     G_prime = nx.convert_node_labels_to_integers(G_prime)
 #     ModularityMatrix = nx.modularity_matrix(G_prime, weight="actual_weight")
     ModularityMatrix = get_modularity_matrix(G_prime, resolution)
     for edge in G_prime.edges():
         G_prime.edges[edge[0], edge[1]]["weight"] = ModularityMatrix[edge[0], edge[1]]
     return G_prime
 
-
-
-
 def find_in_list_of_list(mylist, char):
     for sub_list in mylist:
         if char in sub_list:
             return (mylist.index(sub_list))
     raise ValueError("'{char}' is not in list".format(char = char))
 
-
 def model_to_communities(var_vals, Graph):
     """
     Method that outputs communities with input model variable values and the Graph
     """
     clustered = []
     
     for v in var_vals:
@@ -254,15 +245,14 @@
 
     for c in range(len(group)):
         group[c].sort()
     group.sort()
     
     return group
 
-
 def decluster_communities(group, Graph, isolated_nodes):
     """
     Method to get communities based on the original graph. Note, input Graph is the reduced graph.
     """
     group_declustered = []
     for comm in group:
         new_comm = []
@@ -307,32 +297,21 @@
     communities=[]
 
     #This code lists all sorted triples of nodes (open and closed)
 #     list_of_tuples=list(combinations(np.sort(list((Graph).nodes())),3))
 #     list_of_triads=[list(elem) for elem in list_of_tuples]
     formulation_time_start = time.time()
     list_of_cut_triads=[]
-    
-#     pairs_with_edges = []
-#     pairs_without_edges = []
-#     for i in (Graph).nodes():
-#         for j in range(i+1, len((Graph).nodes())):
-#             if Graph.has_edge(i, j):
-#                 pairs_with_edges.append((i, j))
-#             else:
-#                 pairs_without_edges.append((i, j))
-
     pairs = set(combinations(np.sort(list((Graph).nodes())),2))
     self_edges =set([(i, i) for i in (Graph).nodes()])
     pairs_with_edges = set((Graph).edges()) - self_edges
     pairs_without_edges = pairs - pairs_with_edges
     pairs_without_edges = list(pairs_without_edges)
     pairs_with_edges = list(pairs_with_edges)
         
-# JOBLIB
     with parallel_backend(backend='loky', n_jobs=-1):
         res = Parallel()(delayed(separating_set_parallel)(pair[0], pair[1], Graph) for pair in pairs_without_edges)
     
     list_of_cut_triads = list(chain(*res))
 
     for pair in pairs_with_edges:
         i = pair[0]
@@ -344,55 +323,35 @@
             Graph.remove_edge(i, j)
         minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
         for k in minimum_vertex_cut:
             list_of_cut_triads.append(list(np.sort([i,j,k])))
         if removed_edge:
             Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
 
-            
-#     list_of_cut_triads = []
-#     for i in (Graph).nodes():
-#         for j in range(i+1, len((Graph).nodes())):
-#             removed_edge = False
-#             if Graph.has_edge(i, j):
-#                 removed_edge = True
-#                 attr_dict = Graph.edges[i, j]
-#                 Graph.remove_edge(i, j)
-#             minimum_vertex_cut=minimum_st_node_cut(Graph, i, j)
-#             for k in minimum_vertex_cut:
-#                 list_of_cut_triads.append(list(np.sort([i,j,k])))
-#             if removed_edge:
-#                 Graph.add_edge(i, j, weight=attr_dict["weight"], constrained_modularity=attr_dict["constrained_modularity"], actual_weight=attr_dict["actual_weight"])
-#     return list_of_cut_triads
-    
-    x={}
+    x = {}
 
     model = Model("Modularity maximization")
+    model.setParam(GRB.param.OutputFlag, 0) 
     model.setParam(GRB.param.Method, lp_method)
     model.setParam(GRB.Param.Crossover, 0)
     model.setParam(GRB.Param.Threads, min(64,multiprocessing.cpu_count()))
-    model.setParam(GRB.param.OutputFlag, 0) 
-
 
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             x[(i,j)] = model.addVar(lb=0, ub=1, vtype=GRB.CONTINUOUS, name=str(i)+','+str(j))
 
     model.update()
 
     OFV = 0 
     for i in range(len(Graph.nodes())):
         for j in range(i+1, len(Graph.nodes())):
             OFV += ModularityMatrix[i, j] * (1 - x[(i, j)])
 
     model.setObjective(OFV, GRB.MAXIMIZE)
 
-    print('Adding constraints...')
-#     for [i,j,k] in list_of_triads:
-#     base_constraints = []
     for [i,j,k] in list_of_cut_triads:
         model.addConstr(x[(i,k)] <= x[(i, j)] + x[(j, k)], 'triangle1'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(i,j)] <= x[(i, k)] + x[(j, k)], 'triangle2'+','+str(i)+','+str(j)+','+str(k))
         model.addConstr(x[(j,k)] <= x[(i, j)] + x[(i, k)], 'triangle3'+','+str(i)+','+str(j)+','+str(k))
 #         base_constraints.append('triangle1'+','+str(i)+','+str(j)+','+str(k))
     formulation_time = time.time() - formulation_time_start
 
@@ -400,15 +359,15 @@
 
     # Using a warm start
     # A known partition can be used as a starting point to "warm-start" the algorithm.
     # It can be provided to the model here by giving start values to the decision variables:
     # If this optional step is skipped, you should comment out these five lines
     if warmstart==1:
         #Solution from Combo algorithm to be used as warm-start
-        partition = algorithms.pycombo(Graph[index])
+        partition = algorithms.pycombo(Graph[index], modularity_resolution=resolution)
         community_combo=list(partition.communities)
         for i in (Graph).nodes():
             for j in filter(lambda x: x>i, (Graph).nodes()):
                 if find_in_list_of_list(community_combo,i)==find_in_list_of_list(community_combo,j):
                     x[(i,j)].start = 0
                 else:
                     x[(i,j)].start = 1   
@@ -431,37 +390,37 @@
 
     obj = model.getObjective()
 
 #     objectivevalue = np.round(((2*obj.getValue()+(ModularityMatrix.trace()[0,0]))/np.sum(AdjacencyMatrix)), 8)
     objectivevalue = np.round(((2*obj.getValue()+(ModularityMatrix.trace()))/np.sum(AdjacencyMatrix)), 8)
 
 
-    print('Instance 0',': modularity equals',objectivevalue) 
+#    print('Instance 0',': modularity equals',objectivevalue) 
 
     if (model.NodeCount)**(1/((size)+2*(order))) >= 1:
         effectiveBranchingFactors = ((model.NodeCount)**(1/((size)+2*(order))))  
     
     var_vals = {}
     for var in model.getVars():
         var_vals[var.varName] = var.x
         
     communities = model_to_communities(var_vals, Graph)
 
-    print("Communities: ", communities)
+#    print("Communities: ", communities)
 
     communities_declustered = decluster_communities(communities, Graph, isolated_nodes)
-    print("Communities de-clustered: ", communities_declustered)
+#    print("Communities de-clustered: ", communities_declustered)
 
     
 
-    print("\n")
-    print("Q*:")
-    print(objectivevalue)
+#    print("\n")
+#    print("Q*:")
+#    print(objectivevalue)
 
-    print("solve time:",solveTime)
+#    print("solve time:",solveTime)
     
     return objectivevalue, var_vals, model, list_of_cut_triads, formulation_time, solveTime
 
 
 # In[10]:
 
 
@@ -496,19 +455,19 @@
     objectivevalue = np.round((((2*obj_val)+(ModularityMatrix.trace()))/np.sum(AdjacencyMatrix)), 8)
 
 
     var_vals = {}
     for var in model.getVars():
         var_vals[var.varName] = var.x
 
-    print("\n")
-    print("Q*:")
-    print(objectivevalue)
+#    print("\n")
+#    print("Q*:")
+#    print(objectivevalue)
 
-    print("solve time:",solveTime)
+#    print("solve time:",solveTime)
     
     return objectivevalue, var_vals, model
 
 
 # In[11]:
 
 
@@ -961,15 +920,15 @@
             ModularityMatrix[i, j] = mod
     return ModularityMatrix
 
 
 # In[46]:
 
 
-def bayan(G, threshold=0.001, time_allowed=60, delta=0.5, resolution=1, lp_method=4):
+def bayan(G, threshold=0.001, time_allowed=600, delta=0.7, resolution=1, lp_method=4):
     """
     Run bayan on input Graph while MIP gap > threshold and runtime < time_allowed (default is 60 seconds)
     """
     run_start = time.time()
     preprocessing_time_start = time.time()
     G = create_int_node_names(G)
     G1 = G.copy()
@@ -984,21 +943,21 @@
     order = len(AdjacencyMatrix)
     preprocessing_time = time.time() - preprocessing_time_start
     mod_lp, var_vals, model, list_of_cut_triads, formulation_time, root_lp_time = lp_formulation(Graph, AdjacencyMatrix, ModularityMatrix, size, order, isolated_nodes, lp_method)
 #     return var_vals
     if is_integer_solution(Graph, var_vals):
         return 1, mod_lp, mod_lp, decluster_communities(model_to_communities(var_vals, Graph), Graph, isolated_nodes), preprocessing_time, formulation_time, root_lp_time
     root_combo_time_start = time.time()
-    partition_combo = algorithms.pycombo(Graph, weight="actual_weight")
+    partition_combo = algorithms.pycombo(Graph, weight="actual_weight", modularity_resolution=resolution)
     communities_combo = list(partition_combo.communities)
 #     return communities_combo
     communities_combo_declustered = decluster_communities(communities_combo, Graph, isolated_nodes)
     mod_combo = calculate_modularity(communities_combo_declustered, orig_graph, resolution)
     root_combo_time = time.time() - root_combo_time_start
-    print(mod_combo)
+#    print(mod_combo)
     if mod_lp - mod_combo < threshold:
         return 2, mod_combo, mod_lp, communities_combo_declustered, preprocessing_time, formulation_time, root_combo_time+root_lp_time
     best_bound = mod_lp
     incumbent = mod_combo
     root = Node([], var_vals, Graph, communities_combo_declustered)
     root.set_level(0)
     root.set_bounds(mod_combo, mod_lp)
@@ -1027,15 +986,15 @@
                         return 4, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
                 else:
                     return 5, best_combo.lower_bound, best_lp.upper_bound, best_combo.combo_communities, preprocessing_time, formulation_time, time.time() - solve_start + root_time
             current_node = node
 #             model.reset()
             left_node, right_node = perform_branch(node, model, incumbent, best_bound, Graph, orig_graph, isolated_nodes, list_of_cut_triads, delta, resolution)
             if left_node.close:
-                print("Left node closed")
+                print("Left node is closed")
                 if left_node.is_integer and incumbent <= left_node.upper_bound:
 #                     p_inc = incumbent
                     incumbent = left_node.upper_bound
                     best_combo = left_node
                     nodes_current_level.append(left_node)
                     lower_bounds.append(left_node.lower_bound)
                     upper_bounds.append(left_node.upper_bound)
@@ -1048,15 +1007,15 @@
                 lower_bounds.append(left_node.lower_bound)
                 upper_bounds.append(left_node.upper_bound)
                 current_node.left = left_node
                 left_node.parent = current_node
                 left_node.set_level(current_level)
 
             if right_node.close:
-                print("Right node closed")
+                print("Right node is closed")
                 if right_node.is_integer and incumbent <= right_node.upper_bound:
                     incumbent = right_node.upper_bound
                     best_combo = right_node
                     nodes_current_level.append(right_node)
                     lower_bounds.append(right_node.lower_bound)
                     upper_bounds.append(right_node.upper_bound)
                     current_node.right = right_node
@@ -1085,15 +1044,15 @@
             count += 1
         for val in not_possible_vals:
             upper_bounds.remove(val)
         best_bound = min(upper_bounds + [best_bound])
         for n in nodes_current_level:
             if n.upper_bound == best_bound:
                 best_lp = n
-        print(incumbent, best_bound)
+#        print("Bounds", incumbent, best_bound)
         current_level += 1
         nodes_p_level = []
         for a in nodes_current_level:
             if a.close == False:
                 nodes_p_level.append(a)
         nodes_previous_level = nodes_p_level
         
@@ -1163,15 +1122,15 @@
     Perform the left and right branch on input node
     """
     violated_triples_dict = node.get_violated_triples(list_of_cut_triads)
     prev_fixed_ones = node.get_fixed_ones().copy()
     prev_fixed_zeros = node.get_fixed_zeros().copy()
     #Select triple based on most common nodes with previous triple
     branch_triple = get_best_triple(violated_triples_dict, node, Graph)
-    print(branch_triple)
+#    print(branch_triple)
     print("======== BRANCHING ON " + str(branch_triple) + " ========")
     x_ij = model.getVarByName(str(branch_triple[0]) + "," + str(branch_triple[1]))
     x_jk = model.getVarByName(str(branch_triple[1]) + "," + str(branch_triple[2]))
     x_ik = model.getVarByName(str(branch_triple[0]) + "," + str(branch_triple[2]))
     
     #Left branch x_ij + x_jk + x_ik = 0
     count = 0
@@ -1201,33 +1160,33 @@
         implied_zeros, implied_ones = left_implied(left_fix_ones, left_fix_zeros, branch_triple)
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     left_graph, edges_added = reduce_triple(node.graph, branch_triple, Graph, resolution)
-    left_partition_combo = algorithms.pycombo(left_graph, treat_as_modularity=True)
+    left_partition_combo = algorithms.pycombo(left_graph, treat_as_modularity=True, modularity_resolution=resolution)
     left_communities_combo = list(left_partition_combo.communities)
     left_decluster_combo = decluster_communities(left_communities_combo, left_graph, isolated_nodes)
     left_graph = remove_extra_edges(left_graph, edges_added)
     left_lower_bound = calculate_modularity(left_decluster_combo, original_graph, resolution)
-    print(left_lower_bound)
+#    print(left_lower_bound)
     left_constraints = node.constraints.copy()
     left_constraints.append(branch_triple + (0,))
     left_node = Node(left_constraints, left_var_vals, left_graph, left_decluster_combo)
     left_node.set_bounds(left_lower_bound, left_upper_bound)
         
     if left_upper_bound == -1 and left_var_vals == -1:
         left_node.close_node()
         left_node.set_is_infeasible()
     else:
         left_node.set_fixed_ones(prev_fixed_ones + left_fix_ones + implied_ones)
         left_node.set_fixed_zeros(prev_fixed_zeros + left_fix_zeros + implied_zeros)
         if is_integer_solution(left_graph, left_var_vals):
-            print("IS integer")
+            print("LP solution is integer")
             left_node.set_is_integer()
             left_node.close_node()
         if left_upper_bound <= incumbent:
             left_node.close_node()
             
         
     
@@ -1264,20 +1223,20 @@
         implied_constraints = right_implied(right_fix_zeros, branch_triple)
     
     for i in range(count):
         model.remove(model.getConstrByName('branch_' + str(i)))
     model.update()
     
     right_graph, edges_added = alter_modularity(node.graph, branch_triple, Graph, delta, resolution)
-    right_partition_combo = algorithms.pycombo(right_graph, treat_as_modularity=True)
+    right_partition_combo = algorithms.pycombo(right_graph, treat_as_modularity=True, modularity_resolution=resolution)
     right_communities_combo = list(right_partition_combo.communities)
     right_decluster_combo = decluster_communities(right_communities_combo, right_graph, isolated_nodes)
     right_lower_bound = calculate_modularity(right_decluster_combo, original_graph, resolution)
     right_graph = remove_extra_edges(right_graph, edges_added)
-    print(right_lower_bound)
+#    print(right_lower_bound)
     right_constraints = node.constraints.copy()
     right_constraints.append(branch_triple + (2,))
     right_constraints += implied_constraints
     right_node = Node(right_constraints, right_var_vals, right_graph, right_decluster_combo)
     right_node.set_bounds(right_lower_bound, right_upper_bound)
     
 
@@ -1285,17 +1244,14 @@
     if right_upper_bound == -1 and right_var_vals == -1:
         right_node.close_node()
         right_node.set_is_infeasible()
     else:
         right_node.set_fixed_ones(prev_fixed_ones + right_fix_ones)
         right_node.set_fixed_zeros(prev_fixed_zeros + right_fix_zeros)
         if is_integer_solution(right_graph, right_var_vals):
-            print("IS integer")
+            print("LP solution is integer")
             right_node.set_is_integer()
             right_node.close_node()
         if right_upper_bound <= incumbent:
             right_node.close_node()
     return left_node, right_node
     
-    
-   
-
```

### Comparing `bayanpy-0.5/bayanpy/bayanpy.py` & `bayanpy-0.6/bayanpy/bayanpy.py`

 * *Files identical despite different names*

### Comparing `bayanpy-0.5/setup.py` & `bayanpy-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bayanpy",
-    version="0.5", 
+    version="0.6", 
 description="Bayanpy is a powerful Python library for community detection in complex networks, designed to provide optimal or near-optimal solutions for modularity maximization. It features a highly efficient branch-and-cut algorithm and is backed by Integer Programming (IP) formulations.",
     packages=find_packages(),
     install_requires=["requests",
         "pandas",
         "networkx",
         "numpy",
         "gurobipy",
```

