# Comparing `tmp/graphretrieval-0.1.2.tar.gz` & `tmp/graphretrieval-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.2.tar", last modified: Sun May 19 08:50:19 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.3.tar", last modified: Sun May 19 12:48:53 2024, max compression
```

## Comparing `graphretrieval-0.1.2.tar` & `graphretrieval-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.012166 graphretrieval-0.1.2/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    25088 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 12:48:53.000000 graphretrieval-0.1.3/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:48:53.512722 graphretrieval-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-19 12:48:45.000000 graphretrieval-0.1.3/setup.py
```

### Comparing `graphretrieval-0.1.2/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.3/GraphRetrieval/GraphRetrieval.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from joblib import Parallel, delayed
 from langchain_text_splitters import CharacterTextSplitter
 from openai import OpenAI
 import pickle
 import langchain_core
 import PyPDF2
 from queue import PriorityQueue
+from PIL import Image
+from torchvision import models, transforms
 
 
 class GraphDocument(langchain_core.documents.base.Document):
     def __init__(self, page_content, metadata):
         super().__init__(page_content=page_content, metadata=metadata)
 
     def __repr__(self):
@@ -48,28 +50,14 @@
 
     names: List[str] = Field(
         ...,
         description="All the person, organization, or business entities that "
         "appear in the text",
     )
 
-import os
-import networkx as nx
-from sentence_transformers import SentenceTransformer
-from sklearn.metrics.pairwise import cosine_similarity
-from sklearn.neighbors import NearestNeighbors
-import heapq
-from joblib import Parallel, delayed
-from langchain_text_splitters import CharacterTextSplitter
-from openai import OpenAI
-import pickle
-import langchain_core
-import PyPDF2
-from queue import PriorityQueue
-
 
 class GraphDocument(langchain_core.documents.base.Document):
     def __init__(self, page_content, metadata):
         super().__init__(page_content=page_content, metadata=metadata)
 
     def __repr__(self):
         return f"GraphDocument(page_content='{self.page_content}', metadata={self.metadata})"
@@ -519,7 +507,114 @@
             )
             | prompt
             | self.llm
             | StrOutputParser()
         )
 
         return chain
+
+
+## image rag
+
+class ImageGraphRAG:
+    def __init__(self):
+        self.graph = None
+        self.documents = None
+        self.embeddings = None
+        self.embedding_model = models.resnet50(pretrained=True)
+        self.embedding_model.eval()
+        self.transform = transforms.Compose([
+            transforms.Resize((224, 224)),
+            transforms.ToTensor(),
+            transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]),
+        ])
+        self.retrieval_model = "a_star"
+
+    def image_to_embedding(self, image_path):
+        image = Image.open(image_path).convert('RGB')
+        image = self.transform(image)
+        image = image.unsqueeze(0)  # add batch dimension
+        with torch.no_grad():
+            embedding = self.embedding_model(image).numpy().flatten()
+        return embedding
+
+    def constructGraph(self, image_paths, similarity_threshold=0.5):
+        documents = [GraphDocument(image_path, {"path": image_path}) for image_path in image_paths]
+        embeddings = [self.image_to_embedding(image_path) for image_path in image_paths]
+        graph = nx.Graph()
+
+        def add_edges(i):
+            edges = []
+            for j in range(i , len(documents)):
+                similarity = cosine_similarity([embeddings[i]], [embeddings[j]])[0][0]
+                if similarity > similarity_threshold:
+                    edges.append((i, j, similarity))
+            return edges
+
+        edge_lists = Parallel(n_jobs=-1)(delayed(add_edges)(i) for i in range(len(documents)))
+        edges = [edge for edge_list in edge_lists for edge in edge_list]
+        graph.add_weighted_edges_from(edges)
+
+        self.graph = graph
+        self.documents = documents
+        self.embeddings = np.array(embeddings)
+
+        return graph, documents, embeddings
+
+    def a_star_search_parallel(self, query_image_path, k=5):
+        query_embedding = self.image_to_embedding(query_image_path)
+        pq = [(0, None, 0)]
+        visited = set()
+        similar_nodes = []
+
+        while pq and len(similar_nodes) < k:
+            _, current_node, similarity_so_far = heapq.heappop(pq)
+
+            if current_node is not None:
+                similar_nodes.append((current_node, similarity_so_far))
+
+            compute_similarity_partial = delayed(self.compute_similarity)
+            results = Parallel(n_jobs=-1)(compute_similarity_partial(neighbor, self.graph, query_embedding) for neighbor in (self.graph.neighbors(current_node) if current_node is not None else range(len(self.documents))))
+
+            for result in results:
+                for neighbor, neighbor_similarity in result:
+                    if neighbor not in visited:
+                        priority = -neighbor_similarity
+                        heapq.heappush(pq, (priority, neighbor, similarity_so_far + neighbor_similarity))
+                        visited.add(neighbor)
+
+        return similar_nodes
+
+    def compute_similarity(self, neighbor, graph, query_embedding):
+        neighbor_embedding = self.embeddings[neighbor]
+        neighbor_similarity = cosine_similarity([query_embedding], [neighbor_embedding])[0][0]
+        return [(neighbor, neighbor_similarity)]
+
+    def similarity_search(self, query_image_path, retrieval_model="a_star", k=5):
+        retrieval_model=self.retrieval_model
+        similar_nodes = []
+
+        if retrieval_model == "a_star":
+            similar_indices = [index for index, _ in self.a_star_search_parallel(query_image_path, k)]
+
+        return [self.documents[index] for index in similar_indices]
+
+    def save_db(self, file_path):
+        with open(file_path, 'wb') as file:
+            pickle.dump((self.graph, self.documents, self.embeddings), file)
+            print("saved!")
+
+    def load_db(self, file_path):
+        with open(file_path, 'rb') as file:
+            self.graph, self.documents, self.embeddings = pickle.load(file)
+            print("loaded!")
+
+    def create_graph_from_directory(self, directory_path, similarity_threshold=0.5):
+        image_paths = [os.path.join(directory_path, fname) for fname in os.listdir(directory_path) if fname.lower().endswith(('png', 'jpg', 'jpeg'))]
+        self.graph, self.documents, self.embeddings = self.constructGraph(image_paths, similarity_threshold)
+        print("Graph created Successfully!")
+        return image_paths
+    
+    def visualize_graph(self):
+        pos = nx.spring_layout(self.graph)
+        nx.draw(self.graph, pos, with_labels=True, node_color='skyblue', edge_color='gray', node_size=1000, font_size=10)
+        plt.show() ## use matplotlib
```

### Comparing `graphretrieval-0.1.2/GraphRetrieval.egg-info/PKG-INFO` & `graphretrieval-0.1.3/GraphRetrieval.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.2
+Version: 0.1.3
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
@@ -103,15 +103,15 @@
 
 ### Ingesting Data into Graph
 
 Ingest large text data into the knowledge graph.
 
 ```python
 
-text = "some large text here"
+text = "enter text here"
 
 from langchain_text_splitters import CharacterTextSplitter
 
 text_splitter = CharacterTextSplitter(
     separator="
 
 ",
@@ -136,16 +136,34 @@
 ```python
 
 gr.vector_index = grag
 gr.hybrid = True
 print(gchain.invoke({"question": "Ask your query here"}))
 ```
 
+## Image Graph RAG
+
+Use directories of images for searching similar images.
+
+```python
+image_graph_rag = ImageGraphRAG()
+image_paths = image_graph_rag.create_graph_from_directory('/content/images')
+similar_images = image_graph_rag.similarity_search('/content/images/car.jpg', k=5)
+
+for doc in similar_images:
+    print(doc.metadata["path"])
+```
+
+```python
+image_graph_rag.visualize_graph() # for graph visualization
+```
+
+
+
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
-
```

### Comparing `graphretrieval-0.1.2/PKG-INFO` & `graphretrieval-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GraphRetrieval
-Version: 0.1.2
+Version: 0.1.3
 Summary: Graph retrieval
 Home-page: https://github.com/jayavibhavnk/GraphRetrieval
 Author: JVNK
 Author-email: jaya11vibhav@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 Requires-Dist: langchain_openai
@@ -103,15 +103,15 @@
 
 ### Ingesting Data into Graph
 
 Ingest large text data into the knowledge graph.
 
 ```python
 
-text = "some large text here"
+text = "enter text here"
 
 from langchain_text_splitters import CharacterTextSplitter
 
 text_splitter = CharacterTextSplitter(
     separator="
 
 ",
@@ -136,16 +136,34 @@
 ```python
 
 gr.vector_index = grag
 gr.hybrid = True
 print(gchain.invoke({"question": "Ask your query here"}))
 ```
 
+## Image Graph RAG
+
+Use directories of images for searching similar images.
+
+```python
+image_graph_rag = ImageGraphRAG()
+image_paths = image_graph_rag.create_graph_from_directory('/content/images')
+similar_images = image_graph_rag.similarity_search('/content/images/car.jpg', k=5)
+
+for doc in similar_images:
+    print(doc.metadata["path"])
+```
+
+```python
+image_graph_rag.visualize_graph() # for graph visualization
+```
+
+
+
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
-
```

### Comparing `graphretrieval-0.1.2/README.rst` & `graphretrieval-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.2/setup.py` & `graphretrieval-0.1.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
 ### Ingesting Data into Graph
 
 Ingest large text data into the knowledge graph.
 
 ```python
 
-text = "some large text here"
+text = "enter text here"
 
 from langchain_text_splitters import CharacterTextSplitter
 
 text_splitter = CharacterTextSplitter(
     separator="\n\n",
     chunk_size=1000,
     chunk_overlap=200,
@@ -116,28 +116,46 @@
 ```python
 
 gr.vector_index = grag
 gr.hybrid = True
 print(gchain.invoke({"question": "Ask your query here"}))
 ```
 
+## Image Graph RAG
+
+Use directories of images for searching similar images.
+
+```python
+image_graph_rag = ImageGraphRAG()
+image_paths = image_graph_rag.create_graph_from_directory('/content/images')
+similar_images = image_graph_rag.similarity_search('/content/images/car.jpg', k=5)
+
+for doc in similar_images:
+    print(doc.metadata["path"])
+```
+
+```python
+image_graph_rag.visualize_graph() # for graph visualization
+```
+
+
+
 #### Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss what you would like to change.
 License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 This `README.md` provides an overview of the GraphRetrieval library, installation instructions, and example usage scenarios, with the specified changes to the file path and environment variables sections.
-
 """
 
 setup(
     name='GraphRetrieval',
-    version='0.1.2',
+    version='0.1.3',
     description='Graph retrieval',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
```

