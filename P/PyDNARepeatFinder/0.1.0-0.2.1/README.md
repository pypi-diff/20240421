# Comparing `tmp/pydnarepeatfinder-0.1.0.tar.gz` & `tmp/pydnarepeatfinder-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydnarepeatfinder-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pydnarepeatfinder-0.2.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pydnarepeatfinder-0.1.0.tar` & `pydnarepeatfinder-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/.gitignore
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/LICENSE
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/README.md
--rw-r--r--   0        0        0      453 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/dna_repeat_finder/__init__.py
--rw-r--r--   0        0        0     1557 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/dna_repeat_finder/cli.py
--rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/dna_repeat_finder/colours.py
--rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/dna_repeat_finder/rob_error.py
--rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/dna_repeat_finder/sequences.py
--rw-r--r--   0        0        0     1304 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/src/hello.txt
--rw-r--r--   0        0        0    10043 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/src/repeatFinder.cpp
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/src/repeatFinder.h
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/tests/test.fasta
--rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/version.py
--rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1184 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1091 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3078 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/.gitignore
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/LICENSE
+-rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/README.md
+-rw-r--r--   0        0        0      453 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/__init__.py
+-rw-r--r--   0        0        0     2472 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/cli.py
+-rw-r--r--   0        0        0     1828 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/colours.py
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/rob_error.py
+-rw-r--r--   0        0        0     3503 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/dna_repeat_finder/sequences.py
+-rw-r--r--   0        0        0     1307 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/hello.txt
+-rw-r--r--   0        0        0     9545 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/repeatFinder.cpp
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/src/repeatFinder.h
+-rw-r--r--   0        0        0      212 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/tests/test.fasta
+-rw-r--r--   0        0        0      316 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/version.py
+-rw-r--r--   0        0        0      967 2022-11-09 12:37:21.000000 pydnarepeatfinder-0.2.1/PKG-INFO
```

### Comparing `pydnarepeatfinder-0.1.0/.github/workflows/pylint.yml` & `pydnarepeatfinder-0.2.1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/.github/workflows/python-package.yml` & `pydnarepeatfinder-0.2.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/.github/workflows/python-publish.yml` & `pydnarepeatfinder-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/.gitignore` & `pydnarepeatfinder-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/LICENSE` & `pydnarepeatfinder-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/dna_repeat_finder/cli.py` & `pydnarepeatfinder-0.2.1/dna_repeat_finder/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,48 +5,69 @@
 import sys
 import argparse
 from PyRepeatFinder import find_repeats
 from .sequences import stream_fasta
 
 __author__ = 'Rob Edwards'
 
-def find_dna_repeats(seqid, dna_seq, gap_len=0, verbose=False):
+def find_dna_repeats(seqid, dna_seq, gap_len=0, min_len=0, verbose=False):
     """
     find the repeats in a dna sequence
     """
 
     if verbose:
         print(f"Finding repeats in {seqid} with seq {dna_seq}", file=sys.stderr)
 
-    r = find_repeats(dna_seq, gap_len)
+    # if(!PyArg_ParseTuple(args, "siii", &dna, &gap_len, &output_rep_len, &debug))
+    r = find_repeats(dna_seq, gap_len, min_len, 0)
+
+    ## NOTE: The numbers returned by find_repeats are 1 indexed!!
 
     for rpt in r:
-        rptlen = rpt['first_end']-rpt['first_start']+1
-        data = [seqid, f"Number:{rpt['repeat_number']}", f"Len:{rptlen}",
+        if rpt['first_end'] > rpt['first_start']:
+            start1 = rpt['first_start']-1
+            rptlen1 = rpt['first_end']-rpt['first_start']
+        else:
+            start1 = rpt['first_end']-1
+            rptlen1 = rpt['first_start']-rpt['first_end']
+
+        if rpt['second_end'] > rpt['second_start']:
+            start2 = rpt['second_start']-1
+            rptlen2 = rpt['second_end']-rpt['second_start']
+        else:
+            start2 = rpt['second_end']-1
+            rptlen2 = rpt['second_start']-rpt['second_end']
+
+        seq1 = dna_seq[start1:start1+rptlen1]
+        seq2 = dna_seq[start2:start2+rptlen2]
+        data = [seqid, f"Number:{rpt['repeat_number']}", f"Len1:{rptlen1}",
+                f"Len2:{rptlen2}",
                 rpt['first_start'], rpt['first_end'],
-                rpt['second_start'], rpt['second_end']
+                rpt['second_start'], rpt['second_end'],
+                seq1, seq2
                ]
         print("\t".join(map(str, data)))
 
 
-def repeats_in_fasta(fafile, gaplen, verbose=False):
+def repeats_in_fasta(fafile, gaplen, minlen, verbose=False):
     """
     Find all the repeats in the sequences in a fasta file
     """
     for seqid, seq in stream_fasta(fafile):
         if verbose:
             print(f"Seqid: {seqid}\nSequence: {seq}", file=sys.stderr)
-        find_dna_repeats(seqid, seq, gaplen, verbose)
+        find_dna_repeats(seqid, seq, gaplen, minlen, verbose)
 
 
 def run():
     """
     Command line run for repeat finder
     """
 
     parser = argparse.ArgumentParser(description='Calculate the repeat sequences in a DNA sequence')
     parser.add_argument('-f', help='fasta file of DNA sequences', required=True)
+    parser.add_argument('-m', help='minimum repeat length', type=int, default=11)
     parser.add_argument('-g', help='gap length (default=0)', type=int, default=0)
     parser.add_argument('-v', help='verbose output', action='store_true')
     args = parser.parse_args()
 
-    repeats_in_fasta(args.f, args.g, args.v)
+    repeats_in_fasta(args.f, args.g, args.m, args.v)
```

### Comparing `pydnarepeatfinder-0.1.0/dna_repeat_finder/colours.py` & `pydnarepeatfinder-0.2.1/dna_repeat_finder/colours.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/dna_repeat_finder/rob_error.py` & `pydnarepeatfinder-0.2.1/dna_repeat_finder/rob_error.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/dna_repeat_finder/sequences.py` & `pydnarepeatfinder-0.2.1/dna_repeat_finder/sequences.py`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/pyproject.toml` & `pydnarepeatfinder-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "PyDNARepeatFinder"
-version = "0.01.0"
+version = "0.2.1"
 authors = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
 maintainers = [
   {name = "Rob Edwards", email = "raedwards@gmail.com"}
 ]
 
@@ -37,9 +37,9 @@
 '''
 
 [tool.scikit-build]
 # Setting py-api to "cp37" would build ABI3 wheels for Python 3.7+.  If CPython
 # is less than this value, or on PyPy, this will be ignored.  Setting the api to
 # "py3" or "py2.py3" would build wheels that don't depend on Python (ctypes,
 # etc).
-wheel.py-api = "cp37"
-wheel.packages = []
+# wheel.py-api = "cp37"
+# wheel.packages = []
```

### Comparing `pydnarepeatfinder-0.1.0/src/repeatFinder.cpp` & `pydnarepeatfinder-0.2.1/src/repeatFinder.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,417 +1,429 @@
-#include <Python.h>
-#include <stdio.h>
-#include <string.h>
-#include <stdlib.h>
-#include <assert.h>
-#include <iostream>
-#include <string>
-#include <vector>
-#include "repeatFinder.h"
-
-using namespace std;
-
-#define REPEAT_LEN                    11
-#define HASH_LEN     (1<<(REPEAT_LEN*2))
-
-unsigned INIT_DNA_LEN = 120000000; 
-
-char inputfile[256] = "test.fasta";
-char *dna;
-int converter[128], complement[128];
-int dna_len;
-int output_rep_len = REPEAT_LEN;
-
-vector<int> allrepeats[HASH_LEN];
-struct repeat{
-	int fst;
-	int sec;
-	int len;
-	int seclen;
-	int visited;
-	int exact;
-}R;
-
-vector<repeat> rep;
-int gap_len = 0;//allow gap < gap_len
-
-
-void input()
-{
-	FILE *f;
-	dna = new char[INIT_DNA_LEN+1];
-	if(!dna){
-		printf("Can not allocate memory\n");
-		exit(0);
-	}
-
-	//input dna
-	f = fopen(inputfile, "r");
-	if(f == NULL){
-		printf("Can not find input file %s\n",inputfile);
-		exit(0);
-	}
-	char *my_new_check  [[maybe_unused]] = fgets(dna,INIT_DNA_LEN,f);
-	
-	strcpy(dna,"");
-	while(fscanf(f, "%s", dna+dna_len)==1) {
-		int t = strlen(dna+dna_len);
-		dna_len += t;
-	}
-	fclose(f);
-
-	//cout << dna << endl;
-
-	//printf("dna len = %d\n",dna_len);
-}
-
-int two_bit_encode(int x) {
-    // convert a base to a two bit encode
-    switch(x) {
-        case 65: // A
-        case 97: // a
-            return 0;
-        case 67: // C
-        case 99: // c
-            return 1;
-        case 71: // G
-        case 103: // g
-            return 2;
-        case 84: // T
-        case 116: //t
-            return 3;
-        default:
-            return rand() % 4;
-    }
-}
-
-// find all the 11 length substring and store their start position
-void find_repeats()
-{
-	int key,start,keylen=2*(REPEAT_LEN-1);
-
-	key = 0;
-	for(start = 0;start < REPEAT_LEN; start++) {
-	        // cout << "key: " << key << " (key<<2) " << (key<<2) << " base: "<< dna[start] << " converter " << two_bit_encode((int) dna[start]) << endl;
-			// key = (key<<2) + converter[(int) dna[start]];
-			key = (key<<2) + two_bit_encode((int) dna[start]);
-    }
-	allrepeats[key].push_back(0);
-
-	for(start = 1;start < dna_len-REPEAT_LEN+1; start++)
-	{
-		//key = ((key&((1<<keylen)-1))<< 2) + converter[(int) dna[start+REPEAT_LEN-1]];
-		key = ((key&((1<<keylen)-1))<< 2) + two_bit_encode((int) dna[start+REPEAT_LEN-1]);
-		// cout << "Base: " << dna[start+REPEAT_LEN-1] << " Convert: " << two_bit_encode((int) dna[start+REPEAT_LEN-1]) << " key: " << key << " start: " << start << endl;
-    	allrepeats[key].push_back(start);
-	}
-
-	//find reverse repeat
-	key = 0;
-	for(start = dna_len-1;start >dna_len-1-REPEAT_LEN; start--)
-		// key = (key<<2) + converter[complement[(int) dna[start]]];
-		key = (key<<2) + two_bit_encode(complement[(int) dna[start]]);
-	allrepeats[key].push_back((dna_len-1)*(-1));
-	
-	for(start = dna_len-2;start >REPEAT_LEN-2; start--)
-	{
-		//key= ((key&((1<<keylen)-1))<<2) + converter[complement[(int) dna[start-REPEAT_LEN+1]]];
-		key= ((key&((1<<keylen)-1))<<2) + two_bit_encode(complement[(int) dna[start-REPEAT_LEN+1]]);
-		allrepeats[key].push_back(start*(-1));
-	}
-}
-
-void find_maxlen(int fst, int sec)
-{
-	int i,j,k;
-	//  check whther to compute //
-	
-	if(sec-fst < REPEAT_LEN)
-		return;
-	
-	if (fst >0)
-		if(dna[fst-1] == dna[sec-1])
-			return;
-
-	k=0;
-	for(i = REPEAT_LEN+fst, j = REPEAT_LEN+sec ; i<sec && j<dna_len; i++, j++)
-		if (dna[i] == dna[j])
-			k++;
-		else 
-			break;
-
-	R.fst=fst+1;
-	R.sec=sec+1;
-	R.len=REPEAT_LEN + k;
-	R.seclen = R.len;
-	R.visited = 0;
-	R.exact = 0;
-	rep.push_back(R);
-}
-
-void find_maxlen_rev(int fst, int sec)
-{
-	int i,j,k;
-	
-	sec = sec *(-1);
-	//  check whther to compute //
-	if(sec-fst +1< 2 * REPEAT_LEN)
-		return;
-	
-	if (fst >0 && sec < dna_len-1 )
-		if(dna[fst-1] == complement[(int) dna[sec+1]])
-			return;
-///////////////
-
-	k=0;
-	for(i = REPEAT_LEN+fst, j = sec - REPEAT_LEN ; i<dna_len && j>-1 && i<j; i++, j--)
-		if (dna[i] == complement[(int) dna[j]])
-			k++;
-		else 
-			break;
-	
-	R.fst=fst+1;
-	R.sec=sec*(-1)-1;
-	R.len=REPEAT_LEN + k;
-	R.seclen = R.len;
-	R.visited = 0;
-	R.exact = 0;
-	rep.push_back(R);
-}
-
-void extend_repeats()
-{
-	int i,j,key,keylen=2*(REPEAT_LEN-1);
-
-	key = 0;
-	for(i = 0;i < REPEAT_LEN; i++)
-		// key = (key<<2) + converter[(int) dna[i]];
-		key = (key<<2) + two_bit_encode((int) dna[i]);
-
-	for(j=0;j<(int) allrepeats[key].size();j++)
-		if(allrepeats[key][j]<0)
-			find_maxlen_rev(0,allrepeats[key][j]);
-		else
-			find_maxlen(0,allrepeats[key][j]);
-
-	for(i =1;i<dna_len-REPEAT_LEN+1;i++){
-		//key = ((key&((1<<keylen)-1))<< 2) + converter[(int) dna[i+REPEAT_LEN-1]];
-		key = ((key&((1<<keylen)-1))<< 2) + two_bit_encode((int) dna[i+REPEAT_LEN-1]);
-		for(j=0;j<(int) allrepeats[key].size();j++)
-			if(allrepeats[key][j]<0)
-				find_maxlen_rev(i,allrepeats[key][j]);
-			else
-				find_maxlen(i,allrepeats[key][j]);
-	}
-}
-
-int check_extend(int fst,int n)
-{
-	int i,j = rep[fst].fst + rep[fst].len -1 +n, len = rep.size(),k, head , tail, mid;
-
-	// binery search
-	head = fst+1;
-	tail = len-1;
-    mid = (head +tail)/2;
-	while(rep[mid].fst!= j && head<=tail){
-		mid = (head +tail)/2;
-		if(rep[mid].fst<j)
-			head = mid+1;
-		else
-			tail = mid -1;
-	}
-
-    if (head <= tail)
-        return -1;
-
-    i = mid-1;
-	while(rep[mid].fst == rep[i].fst && i > tail-1)
-		i--;
-	i++;
-////
-	k = rep[fst].sec+rep[fst].seclen -1;
-
-
-    for(; i < (int) rep.size() && rep[i].fst == j;i++) {
-        if (rep[i].visited == 0) {
-            if ((rep[i].fst + rep[i].len - 1) < rep[fst].sec ||
-                (rep[i].fst + rep[i].len - 1) < (rep[i].sec) * (-1) - rep[i].seclen + 1)
-                //check for 2nd copy
-                if (rep[i].sec - k <= gap_len && rep[i].sec - k >= 0)
-                    return i;
-        }
-        std::cerr << " j: " << j << " fst " << rep[i].fst << " i: " << i << " size: " << rep.size() << std::endl;
-    }
-	return -1;
-}
-	
-void extend_gapped_repeat()
-{
-	int i,j,k, len = rep.size();
-	
-	for(i =0;i<len;i++)
-		if(rep[i].visited==0)
-			for(j=1;j<=gap_len;j++){
-				
-				k = check_extend(i,j);
-				if(k==-1)
-					continue;
-			
-				//extend repeat
-				rep[i].len += j+ rep[k].len-1;
-				rep[i].seclen += rep[k].sec -(rep[i].sec+rep[i].seclen -1) + rep[k].seclen-1;
-				rep[i].exact = 1;
-				rep[k].visited = 1;
-				i--;
-				break;
-			}
-}	
-
-void print_output()
-{
-	int i,j;
-	FILE *f;
-	char outputfile[256];
-
-    strcpy (outputfile,inputfile);
-    strcat (outputfile,".repeatfinder");
-    f = fopen(outputfile,"w");
-
-	j = rep.size();
-
-	int totalRep = 0;
-	for(i=0;i<j;i++)
-		if(rep[i].visited==0 && rep[i].len>= output_rep_len){
-			fprintf(f,"%d\t%d\t",rep[i].fst,rep[i].fst+rep[i].len-1);
-			if(rep[i].sec>-1)
-				fprintf(f,"%d\t%d\n",rep[i].sec,rep[i].sec+rep[i].seclen-1);	
-			else
-				fprintf(f,"%d\t%d\n",rep[i].sec*(-1),(rep[i].sec+rep[i].seclen-1)*(-1));
-			totalRep++;
-		}
-	fclose(f);
-}
-
-
-void run() {
-
-	//initialize
-	converter['A']=0;
-	converter['a']=0;
-	converter['C']=1;
-	converter['c']=1;
-	converter['G']=2;
-	converter['g']=2;
-	converter['T']=3;
-	converter['t']=3;
-	complement['A']='T';
-	complement['a']='t';
-	complement['C']='G';
-	complement['c']='g';
-	complement['G']='C';
-	complement['g']='c';
-	complement['T']='A';
-	complement['t']='a';
-
-	find_repeats();
-	extend_repeats();
-
-	gap_len++;
-	//printf("total rep without join = %d\n",rep.size());
-
-	if(gap_len>1)
-		extend_gapped_repeat();
-
-}
-
-
-int main(int argc, char **argv)
-{
-	int i;
-
-	/*if(argc<2){
-		fprintf(stderr, "Command line not valid.\n -f \"fileName\" -g \"Gap Length\"\nUse 0 for no gap\n");
-		exit(0);
-	}*/
-
-	for(i=1;i<argc;i++) {
-		if(!strcmp(argv[i], "-f")  || !strcmp(argv[i], "-F")) {
-			assert(i+1 < argc);
-			strcpy(inputfile, argv[i+1]);
-			i++;
-		}
-		else if(!strcmp(argv[i], "-g")  || !strcmp(argv[i], "-G")) {
-			assert(i+1 < argc);
-			sscanf(argv[i+1], "%d", &gap_len);
-			i++;
-		}
-		/*		else if(!strcmp(argv[i], "-l")  || !strcmp(argv[i], "-L")) {
-			assert(i+1 < argc);
-			sscanf(argv[i+1], "%u", &INIT_DNA_LEN);
-			i++;
-			}*/
-		else if(!strcmp(argv[i], "-l")  || !strcmp(argv[i], "-L")) {
-			assert(i+1 < argc);
-			sscanf(argv[i+1], "%u", &output_rep_len);
-			i++;
-		}
-		else {
-			fprintf(stderr, "Command line not valid. -f \"fileName\" \n-g \"Gap Length\" (Use 0 for not joining) \n-l \"dna length\" (Specify DNA length if its > 10 million)\n");
-			exit(0);
-		}
-	}
-
-	input();
-    run();
-    print_output();
-	return 0;
-}
-
-static PyObject *
-python_input(PyObject *self, PyObject *args) {
-    /* Parse arguments */
-    if(!PyArg_ParseTuple(args, "si", &dna, &gap_len)) {
-        PyErr_SetString(PyExc_RuntimeError, "Could not parse the arguments to python_input");
-        return NULL;
-    }
-    dna_len = strlen(dna);
-    run();
-
-    // incase you need to debug, uncomment these two lines
-    //strcpy(inputfile, "ROBTEST");
-    //print_output();
-
-    // convert our vector of arrays to a Python object
-    Py_ssize_t len = rep.size();
-    PyObject *result = PyList_New(0);
-
-
-    int totalRep = 0;
-	for(int i=0;i<len;i++) {
-		if(rep[i].visited==0 && rep[i].len>= output_rep_len){
-            // we just use a temp variable to deal with the
-            // case when second start < 0
-		    int ss = rep[i].sec;
-		    int se = rep[i].sec+rep[i].seclen-1;
-		    if(rep[i].sec<0) {
-		        ss = rep[i].sec*(-1);
-		        se = (rep[i].sec+rep[i].seclen-1)*(-1);
-		    }
-			totalRep++;
-
-		    PyObject *item = Py_BuildValue("{s:i, s:i,s:i,s:i,s:i}",
-		    "repeat_number", totalRep,
-            "first_start", rep[i].fst,
-            "first_end", rep[i].fst+rep[i].len-1,
-            "second_start", ss,
-            "second_end", se
-            );
-           PyList_Append(result, item);
-           }
-    }
-    return result;
-}
-
-
-PyMODINIT_FUNC PyInit_PyRepeatFinder(void) {
-    return PyModule_Create(&PyRepeatFinderModule);
-}
+#include <Python.h>
+#include <stdio.h>
+#include <string.h>
+#include <stdlib.h>
+#include <assert.h>
+#include <iostream>
+#include <string>
+#include <vector>
+#include "repeatFinder.h"
+
+using namespace std;
+
+#define REPEAT_LEN                    5
+#define HASH_LEN     (1<<(REPEAT_LEN*2))
+
+unsigned INIT_DNA_LEN = 120000000; 
+
+char inputfile[256] = "test.fasta";
+char *dna;
+int complement[128];
+int dna_len;
+int output_rep_len = REPEAT_LEN;
+int debug = 0;
+
+vector<int> allrepeats[HASH_LEN];
+struct repeat{
+	int fst;
+	int sec;
+	int len;
+	int seclen;
+	int visited;
+	int exact;
+}R;
+
+vector<repeat> rep;
+int gap_len = 0; //allow gap < gap_len
+
+
+int two_bit_encode(int x) {
+    // convert a base to a two bit encode
+    switch(x) {
+        case 65: // A
+        case 97: // a
+            return 0;
+        case 67: // C
+        case 99: // c
+            return 1;
+        case 71: // G
+        case 103: // g
+            return 2;
+        case 84: // T
+        case 116: //t
+            return 3;
+        default:
+            return rand() % 4;
+    }
+}
+
+
+
+void input()
+{
+	FILE *f;
+	dna = new char[INIT_DNA_LEN+1];
+	if(!dna){
+		printf("Can not allocate memory\n");
+		exit(0);
+	}
+
+	//input dna
+	f = fopen(inputfile, "r");
+	if(f == NULL){
+		printf("Can not find input file %s\n",inputfile);
+		exit(0);
+	}
+	char *my_new_check = fgets(dna,INIT_DNA_LEN,f);
+	(void) my_new_check; // remove an unused parameter warning
+	
+	strcpy(dna,"");
+	while(fscanf(f, "%s", dna+dna_len)==1) {
+		int t = strlen(dna+dna_len);
+		dna_len += t;
+	}
+	fclose(f);
+
+	//printf("dna len = %d\n",dna_len);
+}
+
+// find all the 11 length substring and store their start position
+void find_repeats()
+{
+	int key,start,keylen=2*(REPEAT_LEN-1);
+
+	key = 0;
+	for(start = 0;start < REPEAT_LEN; start++)
+		key = (key<<2) + two_bit_encode((int) dna[start]);
+	allrepeats[key].push_back(0);
+
+	for(start = 1;start < dna_len-REPEAT_LEN+1; start++)
+	{
+		key = ((key&((1<<keylen)-1))<< 2) + two_bit_encode((int) dna[start+REPEAT_LEN-1]);
+		allrepeats[key].push_back(start);
+	}
+
+	//find reverse repeat
+	key = 0;
+	for(start = dna_len-1;start >dna_len-1-REPEAT_LEN; start--)
+		key = (key<<2) + two_bit_encode(complement[(int) dna[start]]);
+	allrepeats[key].push_back((dna_len-1)*(-1));
+	
+	for(start = dna_len-2;start >REPEAT_LEN-2; start--)
+	{
+		key= ((key&((1<<keylen)-1))<<2) + two_bit_encode(complement[(int) dna[start-REPEAT_LEN+1]]);
+		allrepeats[key].push_back(start*(-1));
+	}
+}
+
+void find_maxlen(int fst, int sec)
+{
+	int i,j,k;
+	//  check whther to compute //
+	
+	if(sec-fst < REPEAT_LEN)
+		return;
+	
+	if (fst >0)
+		if(dna[fst-1] == dna[sec-1])
+			return;
+
+	k=0;
+	for(i = REPEAT_LEN+fst, j = REPEAT_LEN+sec ; i<sec && j<dna_len; i++, j++)
+		if (dna[i] == dna[j])
+			k++;
+		else 
+			break;
+
+    if (debug && sec > dna_len) {
+        fprintf(stderr, "In find_maxlen we added a repeat with sec %d that is longer than dna_len (%d)\n", sec, dna_len);
+    }
+
+	R.fst=fst+1;
+	R.sec=sec+1;
+	R.len=REPEAT_LEN + k;
+	R.seclen = R.len;
+	R.visited = 0;
+	R.exact = 0;
+	rep.push_back(R);
+}
+
+void find_maxlen_rev(int fst, int sec)
+{
+	int i,j,k;
+	
+	sec = sec *(-1);
+	//  check whther to compute //
+	if(sec-fst +1< 2 * REPEAT_LEN)
+		return;
+	
+	if (fst >0 && sec < dna_len-1 )
+		if(dna[fst-1] == complement[(int) dna[sec+1]])
+			return;
+///////////////
+
+	k=0;
+	for(i = REPEAT_LEN+fst, j = sec - REPEAT_LEN ; i<dna_len && j>-1 && i<j; i++, j--)
+		if (dna[i] == complement[(int) dna[j]])
+			k++;
+		else 
+			break;
+	
+	R.fst=fst+1;
+	R.sec=sec*(-1)-1;
+	R.len=REPEAT_LEN + k;
+	R.seclen = R.len;
+	R.visited = 0;
+	R.exact = 0;
+	rep.push_back(R);
+}
+
+void extend_repeats()
+{
+	int i,j,key,keylen=2*(REPEAT_LEN-1);
+
+	key = 0;
+	for(i = 0;i < REPEAT_LEN; i++)
+		key = (key<<2) + two_bit_encode((int) dna[i]);
+	for(j=0; j < (int) allrepeats[key].size(); j++)
+		if(allrepeats[key][j]<0)
+			find_maxlen_rev(0,allrepeats[key][j]);
+		else
+			find_maxlen(0,allrepeats[key][j]);
+
+	for(i =1;i<dna_len-REPEAT_LEN+1;i++){
+		key = ((key&((1<<keylen)-1))<< 2) + two_bit_encode((int) dna[i+REPEAT_LEN-1]);
+		for(j=0; j < (int) allrepeats[key].size(); j++)
+			if(allrepeats[key][j]<0)
+				find_maxlen_rev(i,allrepeats[key][j]);
+			else
+				find_maxlen(i,allrepeats[key][j]);
+	}
+}
+
+int check_extend(int fst,int n)
+{
+	int i,j = rep[fst].fst + rep[fst].len -1 +n, len = rep.size(),k, head , tail, mid;
+
+
+	// binery search
+	head = fst+1;
+	tail = len-1;
+	mid = (head +tail)/2;
+	while(rep[mid].fst!= j && head<=tail){
+		mid = (head +tail)/2;
+		if(rep[mid].fst<j)
+			head = mid+1;
+		else
+			tail = mid-1;
+	}
+
+	if (head <= tail)
+		return -1;
+
+	i = mid-1;
+	// while (rep[mid].fst == rep[i].fst && i >-1)
+	while(rep[mid].fst == rep[i].fst && i > tail-1)
+		i--;
+	i++;
+////
+	k = rep[fst].sec+rep[fst].seclen -1;
+	
+	for(; i < (int) rep.size() && rep[i].fst == j;i++)
+		if(rep[i].visited == 0){
+			if ( (rep[i].fst + rep[i].len -1) <rep[fst].sec || (rep[i].fst + rep[i].len -1)<(rep[i].sec)*(-1)-rep[i].seclen+1)
+				//check for 2nd copy
+				if(rep[i].sec-k <= gap_len && rep[i].sec-k >= 0)
+					return i;
+		}		
+	return -1;
+}
+	
+void extend_gapped_repeat()
+{
+	int i,j,k, len = rep.size();
+	
+	for(i =0;i<len;i++)
+		if(rep[i].visited==0)
+			for(j=1;j<=gap_len;j++){
+				
+				k = check_extend(i,j);
+				if(k==-1)
+					continue;
+			
+				//extend repeat
+				rep[i].len += j+ rep[k].len-1;
+				rep[i].seclen += rep[k].sec -(rep[i].sec+rep[i].seclen -1) + rep[k].seclen-1;
+				rep[i].exact = 1;
+				rep[k].visited = 1;
+				i--;
+				break;
+			}
+}	
+
+
+void write_dna()
+{
+// write the dna sequence we are testing to a file. This is for debugging purposes!
+    FILE *f;
+	char outputfile[300];
+
+    sprintf(outputfile, "%s.prophage.fasta", inputfile);
+    f = fopen(outputfile,"w");
+    fprintf(f, ">repeat\n%s\n", dna);
+    fclose(f);
+}
+
+void print_output()
+{
+	int i,j;
+	FILE *f;
+	char outputfile[300];
+
+
+    sprintf(outputfile, "%s.prophage.repeatfinder", inputfile);
+    f = fopen(outputfile,"w");
+    fprintf(f, "First repeat start\tFirst repeat end\tSecond repeat start\tSecond repeat end\tFirst len\tSecond len\tExact\tVisited\n");
+
+	j = rep.size();
+
+	int totalRep = 0;
+	for(i=0;i<j;i++)
+		if(rep[i].visited==0 && rep[i].len > output_rep_len){
+			fprintf(f,"%d\t%d\t",rep[i].fst,rep[i].fst+rep[i].len-1);
+			if(rep[i].sec>-1)
+				fprintf(f,"%d\t%d",rep[i].sec,rep[i].sec+rep[i].seclen-1);
+			else
+				fprintf(f,"%d\t%d",rep[i].sec*(-1),(rep[i].sec+rep[i].seclen-1)*(-1));
+			fprintf(f, "\t%d\t%d\t%d\t%d\n", rep[i].len, rep[i].seclen, rep[i].exact, rep[i].visited);
+			totalRep++;
+		}
+	fclose(f);
+}
+
+
+void run() {
+
+	//initialize
+	complement[(int) 'A']='T';
+	complement[(int) 'a']='t';
+	complement[(int) 'C']='G';
+	complement[(int) 'c']='g';
+	complement[(int) 'G']='C';
+	complement[(int) 'g']='c';
+	complement[(int) 'T']='A';
+	complement[(int) 't']='a';
+
+	find_repeats();
+	extend_repeats();
+
+	gap_len++;
+	//printf("total rep without join = %d\n",rep.size());
+
+	if(gap_len>1)
+		extend_gapped_repeat();
+
+}
+
+
+int main(int argc, char **argv)
+{
+	int i;
+
+	/*if(argc<2){
+		fprintf(stderr, "Command line not valid.\n -f \"fileName\" -g \"Gap Length\"\nUse 0 for no gap\n");
+		exit(0);
+	}*/
+
+	for(i=1;i<argc;i++) {
+		if(!strcmp(argv[i], "-f")  || !strcmp(argv[i], "-F")) {
+			assert(i+1 < argc);
+			strcpy(inputfile, argv[i+1]);
+			i++;
+		}
+		else if(!strcmp(argv[i], "-g")  || !strcmp(argv[i], "-G")) {
+			assert(i+1 < argc);
+			sscanf(argv[i+1], "%d", &gap_len);
+			i++;
+		}
+		/*		else if(!strcmp(argv[i], "-l")  || !strcmp(argv[i], "-L")) {
+			assert(i+1 < argc);
+			sscanf(argv[i+1], "%u", &INIT_DNA_LEN);
+			i++;
+			}*/
+		else if(!strcmp(argv[i], "-l")  || !strcmp(argv[i], "-L")) {
+			assert(i+1 < argc);
+			sscanf(argv[i+1], "%u", &output_rep_len);
+			i++;
+		}
+		else {
+			fprintf(stderr, "Command line not valid. -f \"fileName\" \n-g \"Gap Length\" (Use 0 for not joining) \n-l \"dna length\" (Specify DNA length if its > 10 million)\n");
+			exit(0);
+		}
+	}
+
+	input();
+    run();
+    print_output();
+    write_dna();
+	return 0;
+}
+
+PyObject *
+python_input(PyObject *self, PyObject *args) {
+    /* Parse arguments */
+    if(!PyArg_ParseTuple(args, "siii", &dna, &gap_len, &output_rep_len, &debug)) {
+        PyErr_SetString(PyExc_RuntimeError, "Could not parse the arguments to python_input");
+        return NULL;
+    }
+    dna_len = strlen(dna);
+    run();
+
+    if (debug) {
+        strcpy(inputfile, "DEBUGGING_REPEATFINDER");
+        print_output();
+        write_dna();
+    }
+
+    // convert our vector of arrays to a Python object
+    Py_ssize_t len = rep.size();
+    PyObject *result = PyList_New(0);
+
+
+    int totalRep = 0;
+	for(int i=0;i<len;i++) {
+		if(rep[i].visited==0 && rep[i].len > output_rep_len){
+            // we just use a temp variable to deal with the
+            // case when second start < 0
+		    int ss = rep[i].sec;
+		    int se = rep[i].sec+rep[i].seclen-1;
+		    if(rep[i].sec<0) {
+		        ss = rep[i].sec*(-1);
+		        se = (rep[i].sec+rep[i].seclen-1)*(-1);
+		    }
+			totalRep++;
+
+		    PyObject *item = Py_BuildValue("{s:i, s:i,s:i,s:i,s:i}",
+		    "repeat_number", totalRep,
+            "first_start", rep[i].fst,
+            "first_end", rep[i].fst+rep[i].len-1,
+            "second_start", ss,
+            "second_end", se
+            );
+	   rep[i].visited=1;
+           PyList_Append(result, item);
+           }
+    }
+
+    // CRITICAL: We need to reset the repeats before we
+    // call this method again from within the same run!
+    for (int i=0; i<HASH_LEN; i++)
+        allrepeats[i].clear();
+
+    rep.clear();
+    return result;
+}
+
+
+PyMODINIT_FUNC PyInit_PyRepeatFinder(void) {
+    return PyModule_Create(&PyRepeatFinderModule);
+}
```

### Comparing `pydnarepeatfinder-0.1.0/src/repeatFinder.h` & `pydnarepeatfinder-0.2.1/src/repeatFinder.h`

 * *Files identical despite different names*

### Comparing `pydnarepeatfinder-0.1.0/PKG-INFO` & `pydnarepeatfinder-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDNARepeatFinder
-Version: 0.1.0
+Version: 0.2.1
 Summary: Rapidly identify repeats in a DNA sequence
 Author-Email: Rob Edwards <raedwards@gmail.com>
 Maintainer-Email: Rob Edwards <raedwards@gmail.com>
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

