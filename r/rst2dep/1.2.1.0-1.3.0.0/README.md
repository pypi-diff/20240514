# Comparing `tmp/rst2dep-1.2.1.0.tar.gz` & `tmp/rst2dep-1.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst2dep-1.2.1.0.tar", last modified: Tue Apr  9 19:17:23 2024, max compression
+gzip compressed data, was "rst2dep-1.3.0.0.tar", last modified: Tue May 14 18:11:23 2024, max compression
```

## Comparing `rst2dep-1.2.1.0.tar` & `rst2dep-1.3.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.998139 rst2dep-1.2.1.0/
--rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.2.1.0/LICENSE
--rw-rw-rw-   0        0        0      762 2024-04-09 19:17:22.997138 rst2dep-1.2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7680 2024-04-09 15:29:13.000000 rst2dep-1.2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.990139 rst2dep-1.2.1.0/rst2dep/
--rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.2.1.0/rst2dep/GUM_academic_census.rs4
--rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.2.1.0/rst2dep/__init__.py
--rw-rw-rw-   0        0        0     3091 2024-04-09 19:13:59.000000 rst2dep-1.2.1.0/rst2dep/__main__.py
--rw-rw-rw-   0        0        0    24689 2023-10-26 19:38:49.000000 rst2dep-1.2.1.0/rst2dep/classes.py
--rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.2.1.0/rst2dep/dep2rst.py
--rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.2.1.0/rst2dep/example.conllu
--rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.2.1.0/rst2dep/example.rs3
--rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.2.1.0/rst2dep/example.rsd
--rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.2.1.0/rst2dep/feature_extraction.py
--rw-rw-rw-   0        0        0     3897 2024-04-09 14:58:00.000000 rst2dep-1.2.1.0/rst2dep/four_units.rs4
--rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.2.1.0/rst2dep/four_units.rsd
--rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.2.1.0/rst2dep/four_units.txt
--rw-rw-rw-   0        0        0    16922 2024-04-09 15:25:37.000000 rst2dep-1.2.1.0/rst2dep/rst2dep.py
--rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.2.1.0/rst2dep/run_tests.py
--rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.2.1.0/rst2dep/salinity_chain.rsd
--rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.2.1.0/rst2dep/salinity_li.rsd
-drwxrwxrwx   0        0        0        0 2024-04-09 19:17:22.996148 rst2dep-1.2.1.0/rst2dep.egg-info/
--rw-rw-rw-   0        0        0      762 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 19:17:22.000000 rst2dep-1.2.1.0/rst2dep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 19:17:22.999138 rst2dep-1.2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      934 2024-04-09 19:13:45.000000 rst2dep-1.2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.987525 rst2dep-1.3.0.0/
+-rw-rw-rw-   0        0        0    10763 2023-06-30 21:19:28.000000 rst2dep-1.3.0.0/LICENSE
+-rw-rw-rw-   0        0        0      762 2024-05-14 18:11:23.986526 rst2dep-1.3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7757 2024-05-14 15:42:10.000000 rst2dep-1.3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.979640 rst2dep-1.3.0.0/rst2dep/
+-rw-rw-rw-   0        0        0    34921 2023-07-20 15:05:40.000000 rst2dep-1.3.0.0/rst2dep/GUM_academic_census.rs4
+-rw-rw-rw-   0        0        0      127 2023-07-05 13:43:17.000000 rst2dep-1.3.0.0/rst2dep/__init__.py
+-rw-rw-rw-   0        0        0     3249 2024-05-14 15:39:31.000000 rst2dep-1.3.0.0/rst2dep/__main__.py
+-rw-rw-rw-   0        0        0    24779 2024-05-14 15:35:46.000000 rst2dep-1.3.0.0/rst2dep/classes.py
+-rw-rw-rw-   0        0        0    16339 2023-07-05 13:43:13.000000 rst2dep-1.3.0.0/rst2dep/dep2rst.py
+-rw-rw-rw-   0        0        0    13395 2021-10-21 19:46:30.000000 rst2dep-1.3.0.0/rst2dep/example.conllu
+-rw-rw-rw-   0        0        0     2902 2021-10-21 20:26:06.000000 rst2dep-1.3.0.0/rst2dep/example.rs3
+-rw-rw-rw-   0        0        0     1368 2021-10-21 20:24:03.000000 rst2dep-1.3.0.0/rst2dep/example.rsd
+-rw-rw-rw-   0        0        0     3234 2023-07-05 14:04:58.000000 rst2dep-1.3.0.0/rst2dep/feature_extraction.py
+-rw-rw-rw-   0        0        0     3897 2024-04-09 14:58:00.000000 rst2dep-1.3.0.0/rst2dep/four_units.rs4
+-rw-rw-rw-   0        0        0      178 2024-02-26 15:37:50.000000 rst2dep-1.3.0.0/rst2dep/four_units.rsd
+-rw-rw-rw-   0        0        0       58 2024-02-26 15:22:18.000000 rst2dep-1.3.0.0/rst2dep/four_units.txt
+-rw-rw-rw-   0        0        0    18783 2024-05-14 18:08:13.000000 rst2dep-1.3.0.0/rst2dep/rst2dep.py
+-rw-rw-rw-   0        0        0      497 2023-06-30 21:52:58.000000 rst2dep-1.3.0.0/rst2dep/run_tests.py
+-rw-rw-rw-   0        0        0    13806 2024-02-27 14:57:34.000000 rst2dep-1.3.0.0/rst2dep/salinity_chain.rsd
+-rw-rw-rw-   0        0        0    13803 2024-02-27 14:57:25.000000 rst2dep-1.3.0.0/rst2dep/salinity_li.rsd
+drwxrwxrwx   0        0        0        0 2024-05-14 18:11:23.985526 rst2dep-1.3.0.0/rst2dep.egg-info/
+-rw-rw-rw-   0        0        0      762 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-14 18:11:23.000000 rst2dep-1.3.0.0/rst2dep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 18:11:23.987525 rst2dep-1.3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      934 2024-05-14 15:41:35.000000 rst2dep-1.3.0.0/setup.py
```

### Comparing `rst2dep-1.2.1.0/LICENSE` & `rst2dep-1.3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/README.md` & `rst2dep-1.3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                         input format
   -d {ltr,rtl,dist}, --depth {ltr,rtl,dist}
                         how to order depth
   -r, --rels            use DEFAULT_RELATIONS for the .rs3 header instead of rels in input data
   -a {li,chain,hirao}, --algorithm {li,chain,hirao}
                         dependency head algorithm (default: li)
   -s, --same_unit       retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain
+  -n, --node_ids        output constituent node IDs in rsd dependency format
 ```
 
 If you have installed the library you can run the converter directly on the commandline with the options you want like this:
 
 ```
 python -m rst2dep -p -f rs3 example.rs3
 ```
```

### Comparing `rst2dep-1.2.1.0/rst2dep/GUM_academic_census.rs4` & `rst2dep-1.3.0.0/rst2dep/GUM_academic_census.rs4`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/__main__.py` & `rst2dep-1.3.0.0/rst2dep/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
                              "a directory xml/ containing additional corpus formats")
     parser.add_argument("-p", "--print", dest="prnt", action="store_true", help="print output instead of serializing to a file")
     parser.add_argument("-f", "--format", choices=["rsd", "conllu", "rs3", "rs4"], default="rs3", help="input format")
     parser.add_argument("-d", "--depth", choices=["ltr", "rtl", "dist"], default="dist", help="how to order depth")
     parser.add_argument("-r", "--rels", action="store_true", help="use DEFAULT_RELATIONS for the .rs3 header instead of rels in input data")
     parser.add_argument("-a","--algorithm",choices=["li","chain","hirao"],help="dependency head algorithm (default: li)",default="li")
     parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain")
+    parser.add_argument("-n","--node_ids",action="store_true",help="output constituent node IDs in rsd dependency format")
 
     options = parser.parse_args()
 
     inpath = options.infiles
 
     if "*" in inpath:
         from glob import glob
@@ -28,15 +29,15 @@
         files = [inpath]
 
     if options.format in ["rs3","rs4"]:
         sys.stderr.write("o Converting from " + options.format + " to rsd format\n")
         for file_ in files:
             sys.stderr.write("Processing " + os.path.basename(file_) + "\n")
 
-            output = make_rsd(file_, options.root, algorithm=options.algorithm, keep_same_unit=options.same_unit)
+            output = make_rsd(file_, options.root, algorithm=options.algorithm, keep_same_unit=options.same_unit, output_const_nid=options.node_ids)
             if options.prnt:
                 print(output)
             else:
                 newname = file_.replace("rs3", "rsd").replace("rs4", "rsd")
                 if newname == file_:
                     newname = file_ + ".rsd"
                 with io.open(newname, 'w', encoding="utf8", newline="\n") as f:
```

### Comparing `rst2dep-1.2.1.0/rst2dep/classes.py` & `rst2dep-1.3.0.0/rst2dep/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             if int(tok.head) < int(self.tokens[0].id):
                 tok.head = "0"
             elif int(tok.head) > int(self.tokens[-1].id):
                 tok.head = "0"
             token_lines.append("|||".join([tok.id,tok.text,tok.lemma,tok.pos,tok.pos,tok.morph,tok.head,tok.func,"_","_"]))
         self.parse = "///".join(token_lines)
 
-    def out_conll(self,feats=False,document_tokens=None):
+    def out_conll(self,feats=False,document_tokens=None, output_const_nid=False):
         self.rebuild_parse()
         head_word = "_"
         if len(self.tokens) == 0:  # No token information
             self.tokens.append(ParsedToken("1","_","_","_","_","0","_"))
         head_func = "_"
 
         if feats:
@@ -140,17 +140,18 @@
             if self.subord in ["LEFT","RIGHT"]:
                 self.subord = "subord=" + self.subord
             feats = "|".join(feat for feat in [first_pos, head_word, head_pos, head_id, head_parent_pos, sent_id, "stype="+self.s_type, "len="+str(len(self.tokens)), head_func, edu_tense, self.subord, self.heading, self.caption, self.para, self.item, self.date] if feat != "_")
             if len(feats)==0:
                 feats = "_"
         else:
             feats = "_"
-
+        top_nid = self.top_nid if output_const_nid else "_"
         signals = ";".join([sig.pretty_print(document_tokens) for sig in self.signals]) if len(self.signals) > 0 else "_"
-        return "\t".join([self.id, self.text, str(self.dist),"_", "_", feats, self.dep_parent, self.dep_rel, "_", signals])
+
+        return "\t".join([self.id, self.text, str(self.dist), top_nid , "_", feats, self.dep_parent, self.dep_rel, "_", signals])
 
     def out_malt(self):
         first = self.tokens[0].lemma
         first_pos = self.tokens[0].pos
         self.rebuild_parse()
         head_word = "_"
         for tok in self.tokens:
```

### Comparing `rst2dep-1.2.1.0/rst2dep/dep2rst.py` & `rst2dep-1.3.0.0/rst2dep/dep2rst.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/example.conllu` & `rst2dep-1.3.0.0/rst2dep/example.conllu`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/example.rs3` & `rst2dep-1.3.0.0/rst2dep/example.rs3`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/example.rsd` & `rst2dep-1.3.0.0/rst2dep/example.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/feature_extraction.py` & `rst2dep-1.3.0.0/rst2dep/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/four_units.rs4` & `rst2dep-1.3.0.0/rst2dep/four_units.rs4`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/rst2dep.py` & `rst2dep-1.3.0.0/rst2dep/rst2dep.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,16 +54,14 @@
     :param exclude: node ID to exclude as target child
     :param block: list of IDs for which children should not be traversed (multinuc right children)
     :param initial_deprel: the original dependency relation of the node triggering the search (needed for algo != li)
     :param algorithm: the algorithm to use for dependency head selection, one of {li,chain,hirao}
     :return: the found child ID or None if none match
     """
 
-    #if nodes[source].left == 43:
-    #    a=4
     if source == "0":
         return None
     else:
         # Check if this is already an EDU
         if nodes[source].kind == "edu" and source != exclude and source not in block:
             return source
         # Loop through children of this node
@@ -139,35 +137,49 @@
     else:
         # direct ancestry
         return 0  # dist
 
 
 def get_nonspan_rel(nodes,node):
     if node.parent == "0":  # Reached the root
-        return "ROOT"
+        return "ROOT_" + node.id
     elif nodes[node.parent].kind == "multinuc" and nodes[node.parent].leftmost_child == node.id:
         return get_nonspan_rel(nodes, nodes[node.parent])
     elif nodes[node.parent].kind == "multinuc" and nodes[node.parent].leftmost_child != node.id:
         return node#.relname
     elif nodes[node.parent].relname != "span":
         grandparent = nodes[node.parent].parent
         if grandparent == "0":
-            return "ROOT"
+            return "ROOT_" + node.id
         elif not (nodes[grandparent].kind == "multinuc" and nodes[node.parent].left == nodes[grandparent].left):
             return nodes[node.parent]#.relname
         else:
             return get_nonspan_rel(nodes,nodes[node.parent])
     else:
         if node.relname.endswith("_r"):
             return node#.relname
         else:
             return get_nonspan_rel(nodes,nodes[node.parent])
 
 
-def make_rsd(rstfile, xml_dep_root,as_text=False, docname=None, out_mode="conll", algorithm="li", keep_same_unit=False):
+def make_rsd(rstfile, xml_dep_root="", as_text=False, docname=None, out_mode="conll", algorithm="li", keep_same_unit=False, output_const_nid=False):
+    """
+    Convert an RST tree to a dependency representation
+
+    :param rstfile: path to an .rs3 or .rs4 file, or a string containing the RST tree if as_text is True
+    :param xml_dep_root: directory containing GUM-style XML files for additional features (use "" if not available)
+    :param as_text: whether rstfile is a string containing the RST tree or a file path
+    :param docname: optional document name to use for output file name
+    :param out_mode: output format, one of {conll,malt}
+    :param algorithm: the algorithm to use for dependency head selection, one of {li,chain,hirao}
+    :param keep_same_unit: if True, retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain
+    :param output_const_nid: use the fourth column in the output to store the constituent tree original node ID for each relation
+    :return: a string containing the dependency representation if as_text is True, otherwise writes to a file
+    """
+
     nodes = read_rst(rstfile,{},as_text=as_text)
 
     text = " ".join([nodes[nid].text for nid in nodes if nodes[nid].kind=="edu"])
     document_tokens = text.split(" ")
 
     # Store any secedge info and remove from nodes
     secedges = []
@@ -238,22 +250,29 @@
             token_reached += edu.token_count
 
     # Get each node with 'span' relation its nearest non-span relname
     for nid in nodes:
         node = nodes[nid]
         new_rel = node.relname
         sigs = []
+        top_nid = nid
         if node.parent == "0":
             new_rel = "ROOT"
         elif node.relname == "span" or (nodes[node.parent].kind == "multinuc" and nodes[node.parent].leftmost_child == nid):
-            new_rel = get_nonspan_rel(nodes,node)
+            new_rel = get_nonspan_rel(nodes, node)
+            if isinstance(new_rel,str):
+                top_nid = new_rel.split("_")[1]
+                new_rel = "ROOT"
+            else:
+                top_nid = new_rel.id
             if new_rel != "ROOT":
                 sigs = new_rel.signals
                 new_rel = new_rel.relname
         node.dep_rel = new_rel
+        node.top_nid = top_nid
         if len(sigs) > 0:
             node.signals = sigs
 
     for nid in nodes:
         node = nodes[nid]
         dep_parent = find_dep_head(nodes, nid, nid, [], node.dep_rel, algorithm=algorithm, keep_same_unit=keep_same_unit)
         if dep_parent is None:
@@ -275,15 +294,14 @@
                     dep_rel = node.dep_rel = "ROOT"
                 else:
                     dep_rel = node.dep_rel = nodes[node.dep_parent].dep_rel
                     node.dep_parent = nodes[node.dep_parent].dep_parent
 
     # Get head EDU and height per node
     node2head_edu = {}
-    node2height = {}
     for edu in edus:
         edu.height = 0
         node = edu
         edu_id = edu.id
         node2head_edu[node.id] = edu_id
         while node.parent != "0":
             this_height = node.height + 1
@@ -310,37 +328,47 @@
 
     out_graph.sort(key=lambda x: int(x.id))
 
     output = []
 
     for node in out_graph:
         if out_mode == "conll":
-            output.append(node.out_conll(feats=feats,document_tokens=document_tokens))
+            output.append(node.out_conll(feats=feats,document_tokens=document_tokens, output_const_nid=output_const_nid))
         else:
             output.append(node.out_malt())
 
     # Insert secedges if any
     src2secedges = collections.defaultdict(set)
+    secedge_mapping = {}
     for secedge in secedges:
         dep_src = node2head_edu[nodes[secedge.source].id]
         dep_trg = node2head_edu[nodes[secedge.target].id]
         src_dist = str(nodes[secedge.source].height)
         trg_dist = str(nodes[secedge.target].height)
         signals = []
         for sig in secedge.signals:
             signals.append(sig.pretty_print(tokens=document_tokens))
         signals = ";".join(sorted(signals)) if len(signals)>0 else "_"
         src2secedges[dep_src].add(":".join([dep_trg,secedge.relname,src_dist,trg_dist,signals]))
+        secedge_mapping[dep_src + "-" + dep_trg] = secedge.id
 
     temp = []
     for i, line in enumerate(output):
         if str(i+1) in src2secedges:
             fields = line.split("\t")
             secstr = "|".join(src2secedges[str(i+1)])
             fields[8] = secstr
+            if output_const_nid:
+                mapping = []
+                for sec in src2secedges[str(i+1)]:
+                    src = fields[0]
+                    trg = sec.split(":")[0]
+                    if src + "-" + trg in secedge_mapping:
+                       mapping.append(src + "-" + trg + ":" + secedge_mapping[src + "-" + trg])
+                    fields[4] = "|".join(mapping)
             line = "\t".join(fields)
         temp.append(line)
 
     output = "\n".join(temp) + "\n"
 
     return output
 
@@ -351,27 +379,28 @@
     parser = ArgumentParser(description=desc)
     parser.add_argument("infiles",action="store",help="file name or glob pattern, e.g. *.rs3")
     parser.add_argument("-c","--corpus_root",action="store",dest="root",default="",help="optional: path to corpus root folder containing a directory dep/ and \n"+
                                                            "a directory xml/ containing additional corpus formats")
     parser.add_argument("-p","--print",dest="prnt",action="store_true",help="print output instead of serializing to a file")
     parser.add_argument("-a","--algorithm",choices=["li","chain","hirao"],help="dependency head algorithm (default: li)",default="li")
     parser.add_argument("-s","--same_unit",action="store_true",help="retain same-unit multinucs in hirao algorithm / attach them as in li algorithm for chain")
+    parser.add_argument("-n","--node_ids",action="store_true",help="output constituent node IDs in rsd dependency format")
 
     options = parser.parse_args()
 
     inpath = options.infiles
 
     if "*" in inpath:
         from glob import glob
         files = glob(inpath)
     else:
         files = [inpath]
 
     for file_ in files:
-        output = make_rsd(file_, options.root, algorithm=options.algorithm, keep_same_unit=options.same_unit)
+        output = make_rsd(file_, options.root, algorithm=options.algorithm, keep_same_unit=options.same_unit, output_const_nid=options.node_ids)
         if options.prnt:
             print(output)
         else:
             newname = file_.replace("rs3", "rsd").replace("rs4", "rsd")
             if newname == file_:
                 newname = file_ + ".rsd"
             with io.open(newname, 'w', encoding="utf8", newline="\n") as f:
```

### Comparing `rst2dep-1.2.1.0/rst2dep/salinity_chain.rsd` & `rst2dep-1.3.0.0/rst2dep/salinity_chain.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep/salinity_li.rsd` & `rst2dep-1.3.0.0/rst2dep/salinity_li.rsd`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/rst2dep.egg-info/SOURCES.txt` & `rst2dep-1.3.0.0/rst2dep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rst2dep-1.2.1.0/setup.py` & `rst2dep-1.3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rst2dep',
   packages = find_packages(),
-  version = '1.2.1.0',
+  version = '1.3.0.0',
   description = 'RST (Rhetorical Structure Theory) constituent and dependency converter for discourse parses',
   author = 'Amir Zeldes',
   author_email = 'amir.zeldes@georgetown.edu',
   package_data = {'':['README.md','LICENSE','requirements.txt'],'rst2dep':['*']},
   install_requires=[],
   url = 'https://github.com/amir-zeldes/rst2dep',
   license='Apache License, Version 2.0',
-  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.2.1.0',
+  download_url = 'https://github.com/amir-zeldes/rst2dep/releases/tag/v1.3.0.0',
   keywords = ['NLP', 'RST', 'discourse', 'dependencies', 'converter', 'conversion','Rhetorical Structure Theory','parsing'],
   classifiers = ['Programming Language :: Python',
 'Programming Language :: Python :: 2',
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: Apache Software License',
 'Operating System :: OS Independent'],
 )
```

