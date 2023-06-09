# Comparing `tmp/pitchcontext-0.1.8.tar.gz` & `tmp/pitchcontext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitchcontext-0.1.8.tar", max compression
+gzip compressed data, was "pitchcontext-0.1.9.tar", max compression
```

## Comparing `pitchcontext-0.1.8.tar` & `pitchcontext-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2022-12-16 21:51:34.158842 pitchcontext-0.1.8/LICENSE
--rw-r--r--   0        0        0     1208 2023-03-17 11:35:54.057500 pitchcontext-0.1.8/README.md
--rw-r--r--   0        0        0      681 2023-04-07 13:15:02.489706 pitchcontext-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9797 2023-04-02 19:11:53.720006 pitchcontext-0.1.8/src/pitchcontext/ComputePitchContext.py
--rw-r--r--   0        0        0     3066 2023-01-25 21:05:35.934401 pitchcontext-0.1.8/src/pitchcontext/PCParameters.py
--rw-r--r--   0        0        0       62 2022-12-16 22:10:25.821160 pitchcontext-0.1.8/src/pitchcontext/__init__.py
--rw-r--r--   0        0        0      852 2023-01-16 19:32:07.285987 pitchcontext-0.1.8/src/pitchcontext/base40.py
--rw-r--r--   0        0        0    32071 2023-04-07 13:13:15.197912 pitchcontext-0.1.8/src/pitchcontext/models.py
--rw-r--r--   0        0        0    16525 2023-03-14 19:18:30.210423 pitchcontext-0.1.8/src/pitchcontext/pitchcontext.py
--rw-r--r--   0        0        0    31046 2023-04-07 12:55:33.025340 pitchcontext-0.1.8/src/pitchcontext/song.py
--rw-r--r--   0        0        0     2304 2023-01-25 15:23:58.099005 pitchcontext-0.1.8/src/pitchcontext/visualize.py
--rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 pitchcontext-0.1.8/setup.py
--rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 pitchcontext-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-16 21:51:34.158842 pitchcontext-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1505 2023-06-09 11:49:37.552041 pitchcontext-0.1.9/README.md
+-rw-r--r--   0        0        0      681 2023-06-09 11:49:45.959725 pitchcontext-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    11796 2023-04-29 19:47:04.283167 pitchcontext-0.1.9/src/pitchcontext/ComputePitchContext.py
+-rw-r--r--   0        0        0     3066 2023-01-25 21:05:35.934401 pitchcontext-0.1.9/src/pitchcontext/PCParameters.py
+-rw-r--r--   0        0        0       62 2022-12-16 22:10:25.821160 pitchcontext-0.1.9/src/pitchcontext/__init__.py
+-rw-r--r--   0        0        0      852 2023-01-16 19:32:07.285987 pitchcontext-0.1.9/src/pitchcontext/base40.py
+-rw-r--r--   0        0        0    32905 2023-05-01 15:16:19.255059 pitchcontext-0.1.9/src/pitchcontext/models.py
+-rw-r--r--   0        0        0    16477 2023-04-11 14:01:51.897299 pitchcontext-0.1.9/src/pitchcontext/pitchcontext.py
+-rw-r--r--   0        0        0    31503 2023-04-12 22:37:31.527563 pitchcontext-0.1.9/src/pitchcontext/song.py
+-rw-r--r--   0        0        0     2304 2023-01-25 15:23:58.099005 pitchcontext-0.1.9/src/pitchcontext/visualize.py
+-rw-r--r--   0        0        0     2473 1970-01-01 00:00:00.000000 pitchcontext-0.1.9/setup.py
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 pitchcontext-0.1.9/PKG-INFO
```

### Comparing `pitchcontext-0.1.8/LICENSE` & `pitchcontext-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pitchcontext-0.1.8/README.md` & `pitchcontext-0.1.9/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 ---
 component-id: pitchcontext
 name: pitchcontext
 description: Python module for melody analysis based on pitch context vectors.
-type: Library
-release-date: 2023-03-15
-release-number: 0.1.4
-work-package: WP3
-pilot: TUNES
+type: SoftwareLibrary
+release-date: 2023-06-02
+release-number: 0.1.9
+work-package: 
+- WP3
+pilot: 
+- TUNES
 keywords:
   - melody
   - pitch analysis
 changelog:
 licence:
 release link:
 --- 
 
 
 # pitchcontext
 Python module for melody analysis based on pitch context vectors.
 
 ## Prerequisites:
-- lilypond installed and in command line path
-- convert (ImageMagick) installed and in command line path
-- kernfiles and corresponding .json files with melodic features
+- lilypond installed and in command line path.
+- convert (ImageMagick) installed and in command line path.
+- kernfiles and corresponding .json files with melodic features.
+
+The .json files need to be formatted according to the standard of [MTCFeatures](https://pvankranenburg.github.io/MTCFeatures/melodyrepresentation.html).
 
 ## Installation
 The latest release of the pitchcontext module can be installed from pypi:
 ```
 $ pip install pitchcontext
 ```
 
@@ -34,15 +38,18 @@
 ```
 $ poetry install
 ```
 This creates a virtual environment with pitchcontext installed.
 
 ## Examples
 Requires a Python3 environment with both pitchcontext and streamlit installed.
-Two examples are provided:
+Four examples are provided:
 - apps/st_dissonance.py
 - apps/st_novelty.py
+- apps/st_unharmonicity.py
+- apps/st_impliedchords.py
 
 To run:
 ```
 $ streamlit run st_dissonance.py -- -krnpath <path_to_kern_files> -jsonpath <path_to_json_files>
 ```
+The -- is needed to pass the following arguments to the python script.
```

### Comparing `pitchcontext-0.1.8/pyproject.toml` & `pitchcontext-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pitchcontext"
-version = "0.1.8"
+version = "0.1.9"
 description = "Library for melody analysis based on pitch context vectors."
 authors = ["Peter van Kranenburg <peter.van.kranenburg@meertens.knaw.nl>"]
 readme = "README.md"
 packages = [{include = "pitchcontext", from = "src"}]
 
 [tool.poetry.dependencies]
 #streamlit is not compatible with Python 3.9.7
```

### Comparing `pitchcontext-0.1.8/src/pitchcontext/ComputePitchContext.py` & `pitchcontext-0.1.9/src/pitchcontext/ComputePitchContext.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,20 +59,61 @@
     def computeContextLengthPre(self, context_ixs):
         pass
 
     @abstractmethod
     def computeContextLengthPost(self, context_ixs):
         pass
 
+class ComputePitchContextExpWindow(ComputePitchContext):
+    def __init__(self, wpc: 'PitchContext'):
+        super().__init__(wpc)
+
+    def computePreContextFixed(self, focus_ix, **context_params_pre):
+        context_pre_ixs = []
+        return context_pre_ixs
+
+    def computePostContextFixed(self, focus_ix, **context_params_post):
+        context_post_ixs = []
+        return context_post_ixs
+
+    def computePreContextAuto(self, focus_ix, **context_params_pre):
+        context_pre_ixs = []
+        return context_pre_ixs
+
+    def computePostContextAuto(self, focus_ix, **context_params_post):
+        context_post_ixs = []
+        return context_post_ixs
+
+    def computeDistanceWeightsPre(self, context_pre_ixs, focus_ix):
+        distance_weights_pre = []
+        return distance_weights_pre
+
+    def computeDistanceWeightsPost(self, context_post_ixs, focus_ix):
+        distance_weights_post = []
+        return distance_weights_post
+
+    def computeContextLength(self, context_ixs):
+        len_context = 0
+        return len_context
+
+    def computeContextLengthPre(self, context_ixs):
+        pass
+
+    def computeContextLengthPost(self, context_ixs):
+        pass
+
+
 class ComputePitchContextScoretime(ComputePitchContext):
     pass
 
+
 class ComputePitchContextNotes(ComputePitchContext):
     pass
 
+
 class ComputePitchContextBeats(ComputePitchContext):
     def __init__(self, wpc: 'PitchContext'):
         super().__init__(wpc)
         #compute some extra features. LENGTH: wpc.ixs
         self.songlength_beat = self.song.mtcsong['features']['beatinsong_float'][wpc.ixs[-1]] + float(Fraction(self.song.mtcsong['features']['beatfraction'][wpc.ixs[-1]])) - self.song.mtcsong['features']['beatinsong_float'][0]
         self.beatinsong = np.array([self.song.mtcsong['features']['beatinsong_float'][ix] for ix in wpc.ixs])
         self.beatinsong_next = np.append(self.beatinsong[1:],self.songlength_beat+self.beatinsong[0]) #first beatinsong might be negative (upbeat)
@@ -184,27 +225,43 @@
     def computeDistanceWeightsPre(self, context_pre_ixs, focus_ix):
         beatoffset_previous = self.beatinsong - self.beatinsong[focus_ix]
         mindist = self.params.min_distance_weight_pre
         len_context_pre = self.computeContextLengthPre(context_pre_ixs)
         distance_weights_pre  = beatoffset_previous[context_pre_ixs] * (1.0-mindist)/len_context_pre + 1.0
         #set negative weights to zero:
         distance_weights_pre[distance_weights_pre<0.0] = 0.0
+        # if focus_ix == 6:
+        #     print("note 6")
+        #     print(f"{beatoffset_previous=}")
+        #     print(f"{mindist=}")
+        #     print(f"{len_context_pre=}")
+        #     print("(1.0-mindist)/len_context_pre = ", (1.0-mindist)/len_context_pre)
+        #     print("pre distance weights for note 6: ", distance_weights_pre)
         return distance_weights_pre
 
     def computeDistanceWeightsPost(self, context_post_ixs, focus_ix):
+        #TODO: make distinction wether focus note is part of context or not.
         beatoffset = self.beatinsong - self.beatinsong[focus_ix]
         slicelength = self.beatinsong_next[focus_ix] - self.beatinsong[focus_ix]
         beatoffset_next = beatoffset - slicelength #set onset of next note to 0.0
         mindist = self.params.min_distance_weight_post
         len_context_post = self.computeContextLengthPost(context_post_ixs)
         distance_weights_post = beatoffset_next[context_post_ixs] * -(1.0-mindist)/len_context_post + 1.0
         #set negative weights to zero:
         distance_weights_post[distance_weights_post<0.0] = 0.0
         #set max weight to one (if focus note in post context, weight of focus note > 1.0)
         distance_weights_post[distance_weights_post>1.0] = 1.0
+        # if focus_ix == 6:
+            # print("note 6")
+            # print(f"{slicelength=}")
+            # print(f"{beatoffset_next=}")
+            # print(f"{mindist=}")
+            # print(f"{len_context_post=}")
+            # print("-(1.0-mindist)/len_context_post = ", -(1.0-mindist)/len_context_post)
+            # print("post distance weights for note 6: ", distance_weights_post)
         return distance_weights_post
 
     def computeContextLength(self, context_ixs):
         if len(context_ixs) > 0:
             len_context = self.beatinsong_next[context_ixs[-1]] - self.beatinsong[context_ixs[0]]
         else:
             len_context = 0.0
```

### Comparing `pitchcontext-0.1.8/src/pitchcontext/PCParameters.py` & `pitchcontext-0.1.9/src/pitchcontext/PCParameters.py`

 * *Files identical despite different names*

### Comparing `pitchcontext-0.1.8/src/pitchcontext/base40.py` & `pitchcontext-0.1.9/src/pitchcontext/base40.py`

 * *Files identical despite different names*

### Comparing `pitchcontext-0.1.8/src/pitchcontext/models.py` & `pitchcontext-0.1.9/src/pitchcontext/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -303,113 +303,87 @@
         self.songlength = self.song.getSongLength()
         self.params = wpc.params  
         self.numchords = 0 # will be set in self.initchords()
         self.chordquality = {} # will be set in self.initchords()
         self.initchords()
 
     def initchords(self):
-        chordmask_dim = np.zeros(40)
-        chordmask_min = np.zeros(40)
-        chordmask_maj = np.zeros(40)
-        chordmask_dom = np.zeros(40)
-        np.put(chordmask_dim, [0, 11, 22], 1.0)
-        np.put(chordmask_min, [0, 11, 23], 1.0)
-        np.put(chordmask_maj, [0, 12, 23], 1.0)
-        np.put(chordmask_dom, [0, 12, 23, 34], 1.0)
+        chordmask_dim = np.zeros(40, dtype=int)
+        chordmask_min = np.zeros(40, dtype=int)
+        chordmask_maj = np.zeros(40, dtype=int)
+        chordmask_dom = np.zeros(40, dtype=int)
+
+        chordmask_dim[[0, 11, 22]] = [1, 3, 5] #[root, third, fifth]
+        chordmask_min[[0, 11, 23]] = [1, 3, 5] #[root, third, fifth]
+        chordmask_maj[[0, 12, 23]] = [1, 3, 5] #[root, third, fifth]
+        chordmask_dom[[0, 12, 23, 34]] = [1, 3, 5, 7] #[root, third, fifth, seventh]
+
         self.chordquality = {
             0: 'dim',
             1: 'm',
             2: '',
             3: '7'
         }
         self.masks = np.stack([chordmask_dim, chordmask_min, chordmask_maj, chordmask_dom])
         self.numchords = self.masks.shape[0]
-
-    def chordTransitionScore(self, chords, chord1_ixs, chord2_ixs, scalemask=np.ones(40, dtype=bool), song=None, wpc=None):
+        self.chordtones = np.zeros((40,40,self.numchords), dtype=int) #(pitch, root of chord, chord quality). 1: root, 3: third, 5: fifth, 7: seventh
+        for chordq in range(self.numchords):
+            for rootpitch in range(40):
+                chordmask_shift = np.roll(self.masks, rootpitch, axis=1)
+                self.chordtones[np.where(chordmask_shift[chordq]),rootpitch,chordq] = chordmask_shift[chordq][np.where(chordmask_shift[chordq])]
+
+    def chordTransitionScore(
+            self,
+            chords,
+            traceback,
+            chord1_ixs,
+            chord2_ixs,
+            scalemask=np.ones(40, dtype=bool),
+            song=None,
+            wpc=None,
+            ih=None
+        ):
+        # Basic implementation
+        # Please, provide your own.
 
         #scoring scheme.
         pitch1 = chord1_ixs[1] % 40
         pitch2 = chord2_ixs[1] % 40
-        songlength = song.songlength
-        shift = (pitch2 - pitch1) % 40 #interval of roots in base40
-
         #no score if root of chord tones is not in the scalemask)
         if not scalemask[pitch1] or not scalemask[pitch2]:
             return 0.0
 
-        #else compute score step by step
-
         # start with score for 'next' chord
         score = chords[chord2_ixs]
-
-        # Discourage same root, different quality #except maj -> dom
-        if pitch1 == pitch2:
-            if chord1_ixs[2] != chord2_ixs[2]:
-                if  not ( chord1_ixs[2] == 2 and chord2_ixs[2] == 3 ):
-                    score = score * 0.1
-
-        # discourage root change on note with low metric weight
-        if song.mtcsong['features']['beatstrength'][chord2_ixs[0]] < 0.5:
-            if pitch1 != pitch2:
-                score = score * 0.5
-
-        # penalty for harmonically distant
-        # HOW TO DO THIS?
-        # e.g. we do not want 
-
-        # prefer root movement of fourth and fifth
-        if shift != 17 and shift != 23 and shift !=0:
-            score = score * 0.8
-
-        # strongly prefer V-I relation for final note
-        if chord2_ixs[0] == songlength - 1:
-            if shift != 17:
-                score = score * 0.5
-
-        # If previous is dom. Then root must be fourth up
-        if chord1_ixs[2] == 3:
-            if shift != 17:
-                score = score * 0.1
-
-        # if root is fourth up: prefer maj or dom for first chord
-        if shift == 17:
-            if chord1_ixs[2] == 0 or chord1_ixs[2] == 1:
-                score = score * 0.8
-
-        #  root or third in melody for last note
-        if chord2_ixs[0] == songlength - 1:
-            melp40 = song.mtcsong['features']['pitch40'][songlength-1] - 1
-            root_int = (melp40 - pitch2) % 40
-            if not root_int in [0, 11, 12]:
-                score = 0.
-
+        
         return score
 
     #ix = ix in full song
     def getP40(self, ix):
         return (self.song.mtcsong['features']['pitch40'][ix] - 1) % 40
 
     # if extendToAllNaturalTones, also include tones that are 'missing'. E.g. NLB070513_01 in G, but no F#
     # include all alterations. So, no F in melody, include Fb, F, and F#
     def getScaleMask(self, extendToAllNaturalTones=False):
 
-        naturals = np.ones(7, dtype=bool) #[F C G D A E B] # True if not seen
+        naturals = np.ones(7, dtype=bool) #[F C G D A E B] # True if stemtone not present in melody
         naturalixs = np.array([19, 2, 25, 8, 31, 14, 37])
         naturalsix = np.zeros(40, dtype=int)
         naturalsix[30:33] = 4 #A
         naturalsix[36:39] = 6 #B
         naturalsix[1:4]   = 1 #C
         naturalsix[7:10]  = 3 #D
         naturalsix[13:16] = 5 #E
         naturalsix[18:21] = 0 #F
         naturalsix[24:27] = 2 #G
 
         seq_length = len(self.wpc.ixs)
 
         #make scalemask for each note. includes the alteration of the stemtone that is CLOSEST to the focus note
+        #TODO: different weight for looking back and looking forward?
 
         #first record at which index the closest same stemtone is in the melody
         mostrecent = np.zeros((seq_length, 7), dtype=int) + 1000 #gives the index of the most recent stemtone (1000 if not yet)
         mostnext = np.zeros((seq_length, 7), dtype=int) - 1000 #gives the index of the closes next occurrence of the scale tone (-1000 if not any more)
         #first pitch for mostrecent
         p40 = self.getP40(self.wpc.ixs[0])
         mostrecent[0][naturalsix[p40]] = 0
@@ -551,45 +525,59 @@
             scalemask = self.getScaleMask(extendToAllNaturalTones=True)
         else:
             scalemask = np.ones((len(self.wpc.ixs), 40), dtype=bool)
         
         chords      = self.getChords(use_scalemask=use_scalemask)
         numpitches  = chords.shape[1]        
         score       = np.zeros( (self.wpc.pitchcontext.shape[0], numpitches, self.numchords) )
-        traceback   = np.zeros( (self.wpc.pitchcontext.shape[0], numpitches, self.numchords, 2), dtype=int ) #coordinates (pitch, chord) for previous chord
+        traceback   = np.zeros( (self.wpc.pitchcontext.shape[0], numpitches, self.numchords, 4), dtype=int ) #coordinates (pitch, chord, ix last root change, previous pitch) for previous chord
         trace       = np.zeros( (self.wpc.pitchcontext.shape[0], 2), dtype=int ) # (pitch, chord) for each note
         trace_score = np.zeros( (self.wpc.pitchcontext.shape[0], 2) ) # (score, score_diff) for each note
 
         #initialization: first note gets its own chords
         score[0] = chords[0]
         for ix in range(1, self.wpc.pitchcontext.shape[0]):
             #find indices of chord1
             chord1_ixs = np.where(chords[ix-1])
             #find indices of chord2
             chord2_ixs = np.where(chords[ix])
-        
+
+            #E.g., NLB191190_01, note 40?
+            #if all available chords are forbidden (score -10.), another chord gets chosen (score 0)
+            #TODO: all chord1_ixs should also be present in chord2_ixs, to always allow continuation of a chord?
+            #TODO: better: only take maximum over scores in chord2_ixs
+
             for ixs2 in zip(chord2_ixs[0], chord2_ixs[1]):
                 allscores = np.zeros( (numpitches, self.numchords) )
                 for ixs1 in zip(chord1_ixs[0], chord1_ixs[1]):
                     transistionscore = chordTransitionScoreFunction(
                         chords,
+                        traceback,
                         (ix-1,ixs1[0],ixs1[1]),
                         (ix, ixs2[0], ixs2[1]),
                         scalemask=scalemask[ix],
                         song=self.song,
-                        wpc=self.wpc
+                        wpc=self.wpc,
+                        ih=self,
                     )
                     allscores[ixs1] = score[ix-1, ixs1[0], ixs1[1]] + transistionscore
                 #now find max
                 max_ixs = np.unravel_index(np.argmax(allscores), allscores.shape)
                 maxscore = allscores[max_ixs]
                 #update score
                 score[ix, ixs2[0], ixs2[1]] = maxscore
                 #update traceback
-                traceback[ix, ixs2[0], ixs2[1]] = max_ixs                
+                traceback[ix, ixs2[0], ixs2[1]][0:2] = max_ixs
+                if ixs2[0] % 40 != max_ixs[0] % 40: #new root @ ix
+                    traceback[ix, ixs2[0], ixs2[1]][2] = ix
+                    traceback[ix, ixs2[0], ixs2[1]][3] = max_ixs[0]
+                else:
+                    traceback[ix, ixs2[0], ixs2[1]][2] = traceback[ix-1, max_ixs[0], max_ixs[1]][2]  #take start of root from prvious in trace
+                    traceback[ix, ixs2[0], ixs2[1]][3] = traceback[ix-1, max_ixs[0], max_ixs[1]][3]  #take previous pitch from prvious in trace
+
 
         #now do the traceback.
         #find max score for last note
         max_ixs = np.unravel_index(np.argmax(score[-1]), score[-1].shape)
         trace[-1] = (max_ixs[0], max_ixs[1])
         trace_score[-1] = (score[-1,max_ixs[0], max_ixs[1]], 0)
         for ix in range(self.wpc.pitchcontext.shape[0]-2, -1, -1):
@@ -599,16 +587,19 @@
             trace_score[ix][0] = thisscore
 
         for ix in range(1, self.wpc.pitchcontext.shape[0]):
             trace_score[ix][1] = trace_score[ix][0] - trace_score[ix-1][0]
 
         return trace, trace_score, score, traceback
 
-    def trace2str(self, trace):
-        return [base40[trace[ix][0]%40] + self.chordquality[trace[ix][1]] for ix in range(self.wpc.pitchcontext.shape[0])]
+    def trace2str(self, trace, contextType=False):
+        if contextType:
+            return [base40[trace[ix][0]%40] + self.chordquality[trace[ix][1]] + str(int(trace[ix][0]/40)) for ix in range(self.wpc.pitchcontext.shape[0])]
+        else:
+            return [base40[trace[ix][0]%40] + self.chordquality[trace[ix][1]] for ix in range(self.wpc.pitchcontext.shape[0])]
 
     def getChords(self, use_scalemask=True):
         seq_length = len(self.wpc.ixs)
         #prepare data structure:
         if use_scalemask:
             scalemask = self.getScaleMask(extendToAllNaturalTones=True)
         else:
@@ -626,49 +617,50 @@
     def getChordsForNote(self, pitchcontextvector, normalize=True, scalemask=np.ones(40, dtype=bool)):
         #find out whether pitches could be arranged as series of thirds
         
         epsilon = 10e-4
         chordmask_minseventh = np.zeros(40)
         np.put(chordmask_minseventh, [34], 1.0) #used for check presence seventh in dom chord
 
-
-
-        #only take natural tones, and one b or one # as root
+        #only take natural tones, one b or one # as root
         valid_shifts = [1, 2, 3, 7, 8, 9, 13, 14, 15, 18, 19, 20, 24, 25, 26, 30, 31, 32, 36, 37, 38]
 
+        #self.masks contains integers indicating the function of the tone in the chord (root, third, fifht, seventh)
+        #here we need masks with ones everywhere
+        binarymasks = np.clip(self.masks, 0, 1)
+
         #get a value for every rotation of the chordmasks
         score_pre = np.zeros((40, self.numchords))
         score_post = np.zeros((40, self.numchords))
         score_all = np.zeros((40, self.numchords))
         strength_pre = np.zeros((40, self.numchords))
         strength_post = np.zeros((40, self.numchords))
         strength_all = np.zeros((40, self.numchords))
         for shift in range(40):
             if not shift in valid_shifts:
                 continue
 
-            chordmask_shift = np.roll(self.masks, shift, axis=1)
+            chordmask_shift = np.roll(binarymasks, shift, axis=1)
             chordmask_minseventh_shift = np.roll(chordmask_minseventh, shift)
 
-            #only accept chords which have all notes in the scale (might fail when scale tones do not occur in the melody e.g. NLB070513_01 in G, but no F#)
+            #only accept chords which have all notes in the (local) scale
             for maskid in range(self.numchords):
                 if np.prod(scalemask[np.where(chordmask_shift[maskid])]) < epsilon:
                     chordmask_shift[maskid] = 0
 
             score_pre[shift] = np.sum(np.multiply(pitchcontextvector[:40],chordmask_shift), axis=1)
             if np.sum(pitchcontextvector[:40]) > epsilon:
                 strength_pre[shift] = score_pre[shift] / np.sum(pitchcontextvector[:40])
             score_post[shift] = np.sum(np.multiply(pitchcontextvector[40:],chordmask_shift), axis=1)
             if np.sum(pitchcontextvector[40:]) > epsilon:
                 strength_post[shift] = score_post[shift] / np.sum(pitchcontextvector[40:])
             score_all[shift] = np.sum(np.multiply(pitchcontextvector[:40]+pitchcontextvector[40:],chordmask_shift), axis=1)
             if np.sum(pitchcontextvector) > epsilon:
                 strength_all[shift] = score_all[shift] / np.sum(pitchcontextvector)
 
-
             #if seventh in dom chord is not present -> erase dom chord
             if np.sum(np.multiply(chordmask_minseventh_shift,pitchcontextvector[:40])) < epsilon:
                 score_pre[shift][3] = 0.0
                 strength_pre[shift][3] = 0.0
             if np.sum(np.multiply(chordmask_minseventh_shift,pitchcontextvector[40:])) < epsilon:
                 score_post[shift][3] = 0.0
                 strength_post[shift][3] = 0.0
@@ -685,41 +677,41 @@
                 score_all  = score_all / np.max(score_all)
 
         scores    = np.concatenate( (score_pre, score_post, score_all) )
         strengths = np.concatenate( (strength_pre, strength_post, strength_all) )
 
         return scores, strengths
     
-    def printChordsForNote(self, scores, strengths):
+    def printChordsForNote(self, chords):
         epsilon = 10e-4
-        chordixs = np.where(scores > epsilon)
+        chordixs = np.where(chords > epsilon)
         chords_pre = []
         chords_post = []
         chords_all = []
 
         for ix in zip(chordixs[0], chordixs[1]):
-            info = (base40[ix[0] % 40], self.chordquality[ix[1]], scores[ix], strengths[ix], scores[ix] * strengths[ix])
+            info = (base40[ix[0] % 40], self.chordquality[ix[1]], chords[ix])
             if ix[0] < 40:
                 chords_pre.append(info)
             else:
                 if ix[0] < 80:
                     chords_post.append(info)
                 else:
                     chords_all.append(info)
         
         print('pre:')
-        for info in sorted(chords_pre, key=lambda x: x[4], reverse=True):
+        for info in sorted(chords_pre, key=lambda x: x[2], reverse=True):
             print(info)
 
         print('post:')
-        for info in sorted(chords_pre, key=lambda x: x[4], reverse=True):
+        for info in sorted(chords_pre, key=lambda x: x[2], reverse=True):
             print(info)
 
         print('all:')
-        for info in sorted(chords_pre, key=lambda x: x[4], reverse=True):
+        for info in sorted(chords_pre, key=lambda x: x[2], reverse=True):
             print(info)
 
     def printChord(self, chord_in):
         chordixs = np.where(chord_in > 0)
         chords = []
         
         for ix in zip(chordixs[0], chordixs[1]):
@@ -780,7 +772,21 @@
                     side2,
                     transistionscore,
                     scores[ix1, ixs1[0], ixs1[1]],
                     transistionscore + scores[ix1, ixs1[0], ixs1[1]],
                 ))
         for tr in sorted(transitions, key=lambda x: x[9], reverse=True):
             print(' '.join([str(t) for t in tr]))
+
+    def printTrace(self, trace, traceback):
+        for ix, tr in enumerate(trace):
+            print(
+                ix,
+                base40[trace[ix][0]%40],
+                self.chordquality[trace[ix][1]],
+                traceback[
+                    ix,
+                    trace[ix][0],
+                    trace[ix][1]
+                ]
+            )
+
```

### Comparing `pitchcontext-0.1.8/src/pitchcontext/pitchcontext.py` & `pitchcontext-0.1.9/src/pitchcontext/pitchcontext.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,14 @@
         start_onsets = [onsettick[ix] for ix in ixs]
         stop_onsets = [song['features']['offsettick'][ix] for ix in ixs]
 
         if accumulateWeight:
             if syncopes:
                 syncopes=False
                 print("Warning: setting accumulateWeight implies syncopes=False.")
-            max_onset = len(beatstrengthgrid)-1
             #for each note make span of onsets:
             for ix, span in enumerate(zip(start_onsets, stop_onsets)):
                 weights[ix] = sum(beatstrengthgrid[span[0]:span[1]])
         else:
             weights = [beatstrength[ix] for ix in ixs]
         
         if syncopes:
```

### Comparing `pitchcontext-0.1.8/src/pitchcontext/song.py` & `pitchcontext-0.1.9/src/pitchcontext/song.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,16 +468,17 @@
         """Create a new music21 stream with notes colored according to `colordict`.
 
         Parameters
         ----------
         colordict : dict
             The keys are the colors, the values the indices of the notes with that color. E.g. {'red':[0,10,11],'grey':[-1]}
             colors notes at indices 0, 10, and 11 red, and the last note grey.
-        lyrics : list (str)
-            Use the items in this list as lyrics
+        lyrics : list (str) OR list of lists (str)
+            Use the items in this list as lyrics, one string for each note.
+            If a list of lists is provided, these will be printed as different lines of lyrics.
         lyrics_ixs : list (int)
             If given, put the lyrics at the given indices in the song. Should have the same length as lyrics.
             If not given, lyrics should have the same length as the song.
 
         Returns
         -------
         music21 Stream
@@ -504,22 +505,30 @@
             else:
                 print('Provide indices for the lyrics')
                 for ix, n in enumerate(s.flat.notes):
                     n.lyric = None
                 return s
         #make sure it is a list (to use .index)
         lyrics_ixs = list(lyrics_ixs)
-
+        #are more lines of lyrics provided?
+        multipleLines = False
+        if lyrics != None:
+            if type(lyrics[0]) == list:
+                multipleLines = True
         for ix, n in enumerate(s.flat.notes):
             n.lyric = None
             try:
                 lyricix = lyrics_ixs.index(ix)
             except ValueError:
                 continue
-            n.addLyric(lyrics[lyricix])
+            if multipleLines:
+                for line in lyrics:
+                    n.addLyric(line[lyricix])
+            else:
+                n.addLyric(lyrics[lyricix])
         return s
     
     #we need to repair lily generated by m21 concerning color
     #\override Stem.color -> \once\override Stem.color
     #\override NoteHead.color -> \once\override NoteHead.color
 
     def repairLyline(self, line):
```

### Comparing `pitchcontext-0.1.8/src/pitchcontext/visualize.py` & `pitchcontext-0.1.9/src/pitchcontext/visualize.py`

 * *Files identical despite different names*

### Comparing `pitchcontext-0.1.8/setup.py` & `pitchcontext-0.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'matplotlib>=3.3,<4.0',
  'music21>=8.0,<9.0',
  'numpy>=1.19,<2.0',
  'seaborn>=0.12.1,<0.13.0']
 
 setup_kwargs = {
     'name': 'pitchcontext',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Library for melody analysis based on pitch context vectors.',
-    'long_description': '---\ncomponent-id: pitchcontext\nname: pitchcontext\ndescription: Python module for melody analysis based on pitch context vectors.\ntype: Library\nrelease-date: 2023-03-15\nrelease-number: 0.1.4\nwork-package: WP3\npilot: TUNES\nkeywords:\n  - melody\n  - pitch analysis\nchangelog:\nlicence:\nrelease link:\n--- \n\n\n# pitchcontext\nPython module for melody analysis based on pitch context vectors.\n\n## Prerequisites:\n- lilypond installed and in command line path\n- convert (ImageMagick) installed and in command line path\n- kernfiles and corresponding .json files with melodic features\n\n## Installation\nThe latest release of the pitchcontext module can be installed from pypi:\n```\n$ pip install pitchcontext\n```\n\nThe development version can be installed by cloning the repository and by using the provided pyproject.toml and poetry. In root of the rep do:\n```\n$ poetry install\n```\nThis creates a virtual environment with pitchcontext installed.\n\n## Examples\nRequires a Python3 environment with both pitchcontext and streamlit installed.\nTwo examples are provided:\n- apps/st_dissonance.py\n- apps/st_novelty.py\n\nTo run:\n```\n$ streamlit run st_dissonance.py -- -krnpath <path_to_kern_files> -jsonpath <path_to_json_files>\n```\n',
+    'long_description': '---\ncomponent-id: pitchcontext\nname: pitchcontext\ndescription: Python module for melody analysis based on pitch context vectors.\ntype: SoftwareLibrary\nrelease-date: 2023-06-02\nrelease-number: 0.1.9\nwork-package: \n- WP3\npilot: \n- TUNES\nkeywords:\n  - melody\n  - pitch analysis\nchangelog:\nlicence:\nrelease link:\n--- \n\n\n# pitchcontext\nPython module for melody analysis based on pitch context vectors.\n\n## Prerequisites:\n- lilypond installed and in command line path.\n- convert (ImageMagick) installed and in command line path.\n- kernfiles and corresponding .json files with melodic features.\n\nThe .json files need to be formatted according to the standard of [MTCFeatures](https://pvankranenburg.github.io/MTCFeatures/melodyrepresentation.html).\n\n## Installation\nThe latest release of the pitchcontext module can be installed from pypi:\n```\n$ pip install pitchcontext\n```\n\nThe development version can be installed by cloning the repository and by using the provided pyproject.toml and poetry. In root of the rep do:\n```\n$ poetry install\n```\nThis creates a virtual environment with pitchcontext installed.\n\n## Examples\nRequires a Python3 environment with both pitchcontext and streamlit installed.\nFour examples are provided:\n- apps/st_dissonance.py\n- apps/st_novelty.py\n- apps/st_unharmonicity.py\n- apps/st_impliedchords.py\n\nTo run:\n```\n$ streamlit run st_dissonance.py -- -krnpath <path_to_kern_files> -jsonpath <path_to_json_files>\n```\nThe -- is needed to pass the following arguments to the python script.\n',
     'author': 'Peter van Kranenburg',
     'author_email': 'peter.van.kranenburg@meertens.knaw.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `pitchcontext-0.1.8/PKG-INFO` & `pitchcontext-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitchcontext
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for melody analysis based on pitch context vectors.
 Author: Peter van Kranenburg
 Author-email: peter.van.kranenburg@meertens.knaw.nl
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,35 +17,39 @@
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
 Description-Content-Type: text/markdown
 
 ---
 component-id: pitchcontext
 name: pitchcontext
 description: Python module for melody analysis based on pitch context vectors.
-type: Library
-release-date: 2023-03-15
-release-number: 0.1.4
-work-package: WP3
-pilot: TUNES
+type: SoftwareLibrary
+release-date: 2023-06-02
+release-number: 0.1.9
+work-package: 
+- WP3
+pilot: 
+- TUNES
 keywords:
   - melody
   - pitch analysis
 changelog:
 licence:
 release link:
 --- 
 
 
 # pitchcontext
 Python module for melody analysis based on pitch context vectors.
 
 ## Prerequisites:
-- lilypond installed and in command line path
-- convert (ImageMagick) installed and in command line path
-- kernfiles and corresponding .json files with melodic features
+- lilypond installed and in command line path.
+- convert (ImageMagick) installed and in command line path.
+- kernfiles and corresponding .json files with melodic features.
+
+The .json files need to be formatted according to the standard of [MTCFeatures](https://pvankranenburg.github.io/MTCFeatures/melodyrepresentation.html).
 
 ## Installation
 The latest release of the pitchcontext module can be installed from pypi:
 ```
 $ pip install pitchcontext
 ```
 
@@ -53,16 +57,19 @@
 ```
 $ poetry install
 ```
 This creates a virtual environment with pitchcontext installed.
 
 ## Examples
 Requires a Python3 environment with both pitchcontext and streamlit installed.
-Two examples are provided:
+Four examples are provided:
 - apps/st_dissonance.py
 - apps/st_novelty.py
+- apps/st_unharmonicity.py
+- apps/st_impliedchords.py
 
 To run:
 ```
 $ streamlit run st_dissonance.py -- -krnpath <path_to_kern_files> -jsonpath <path_to_json_files>
 ```
+The -- is needed to pass the following arguments to the python script.
```

