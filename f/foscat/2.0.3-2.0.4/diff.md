# Comparing `tmp/foscat-2.0.3.tar.gz` & `tmp/foscat-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-luhq8ofd/foscat-2.0.3.tar", last modified: Thu May 11 14:32:20 2023, max compression
+gzip compressed data, was "/export/home/jmdeloui/FOSCAT/dist/.tmp-32znl1a1/foscat-2.0.4.tar", last modified: Wed Jul  5 08:43:24 2023, max compression
```

## Comparing `foscat-2.0.3.tar` & `foscat-2.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 14:32:20.000000 foscat-2.0.3/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-11 14:32:20.000000 foscat-2.0.3/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.3/README.md
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-05-11 14:32:20.000000 foscat-2.0.3/setup.cfg
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-05-11 14:31:36.000000 foscat-2.0.3/setup.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 14:32:20.000000 foscat-2.0.3/src/
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57131 2023-05-02 14:56:56.000000 foscat-2.0.3/src/foscat/FoCUS.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.3/src/foscat/GetGPUinfo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1766 2023-03-31 09:38:33.000000 foscat-2.0.3/src/foscat/Rformat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    15268 2023-05-11 10:09:32.000000 foscat-2.0.3/src/foscat/Synthesis.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.3/src/foscat/__init__.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13465 2023-03-31 07:45:21.000000 foscat-2.0.3/src/foscat/backend.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.3/src/foscat/build_demo.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.3/src/foscat/demo2d.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    21467 2023-05-02 15:09:32.000000 foscat-2.0.3/src/foscat/scat.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.3/src/foscat/scat_cov.old.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    46094 2023-05-11 10:27:00.000000 foscat-2.0.3/src/foscat/scat_cov.py
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.3/src/foscat/scat_cov_new.py
-drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/PKG-INFO
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/SOURCES.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/dependency_links.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/requires.txt
--rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-05-11 14:32:20.000000 foscat-2.0.3/src/foscat.egg-info/top_level.txt
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 08:43:24.000000 foscat-2.0.4/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     2160 2022-12-13 16:07:53.000000 foscat-2.0.4/README.md
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      107 2023-07-05 08:43:24.000000 foscat-2.0.4/setup.cfg
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     1097 2023-07-05 08:42:27.000000 foscat-2.0.4/setup.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    57132 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/FoCUS.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      731 2023-01-27 14:00:55.000000 foscat-2.0.4/src/foscat/GetGPUinfo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)     3594 2023-06-23 10:27:41.000000 foscat-2.0.4/src/foscat/Rformat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    16208 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/Synthesis.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2022-12-13 16:07:53.000000 foscat-2.0.4/src/foscat/__init__.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    13733 2023-06-10 06:53:35.000000 foscat-2.0.4/src/foscat/backend.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    53863 2023-03-28 12:51:05.000000 foscat-2.0.4/src/foscat/build_demo.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        0 2023-03-04 09:58:28.000000 foscat-2.0.4/src/foscat/demo2d.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    29024 2023-07-05 08:23:52.000000 foscat-2.0.4/src/foscat/scat.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    41808 2023-03-24 11:01:28.000000 foscat-2.0.4/src/foscat/scat_cov.old.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    48336 2023-07-05 08:21:43.000000 foscat-2.0.4/src/foscat/scat_cov.py
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)    27568 2023-02-08 17:11:11.000000 foscat-2.0.4/src/foscat/scat_cov_new.py
+drwxr-xr-x   0 jmdeloui (64609) lpo      (10731)        0 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      751 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/PKG-INFO
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)      475 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/SOURCES.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        1 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/dependency_links.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)       55 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/requires.txt
+-rw-r--r--   0 jmdeloui (64609) lpo      (10731)        7 2023-07-05 08:43:24.000000 foscat-2.0.4/src/foscat.egg-info/top_level.txt
```

### Comparing `foscat-2.0.3/PKG-INFO` & `foscat-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.3
+Version: 2.0.4
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

### Comparing `foscat-2.0.3/README.md` & `foscat-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `foscat-2.0.3/setup.py` & `foscat-2.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='foscat',
-    version='2.0.3',
+    version='2.0.4',
     description='Generate synthetic Healpix or 2D data using Cross Scattering Transform' ,
     long_description='Utilize the Cross Scattering Transform (described in https://arxiv.org/abs/2207.12527) to synthesize Healpix or 2D data that is suitable for component separation purposes, such as denoising. \n A demo package for this process can be found at https://github.com/jmdelouis/FOSCAT_DEMO. \n\n List of developers : J.-M. Delouis, T. Foulquier, L. Mousset, E. Allys ' ,
     license='MIT',
     author='Jean-Marc DELOUIS',
     author_email='jean.marc.delouis@ifremer.fr',
     maintainer='Theo Foulquier',
     maintainer_email='theo.foulquier@ifremer.fr',
```

### Comparing `foscat-2.0.3/src/foscat/FoCUS.py` & `foscat-2.0.4/src/foscat/FoCUS.py`

 * *Files 0% similar despite different names*

```diff
@@ -1349,11 +1349,12 @@
         for i in range(c.shape[1]):
             plt.subplot(2,c.shape[1],1+i)
             plt.imshow(c[:,i].reshape(npt,npt),cmap='jet',vmin=-c.max(),vmax=c.max())
             plt.subplot(2,c.shape[1],1+i+c.shape[1])
             plt.imshow(s[:,i].reshape(npt,npt),cmap='jet',vmin=-c.max(),vmax=c.max())
             sys.stdout.flush()
         plt.show()
+
```

### Comparing `foscat-2.0.3/src/foscat/GetGPUinfo.py` & `foscat-2.0.4/src/foscat/GetGPUinfo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.3/src/foscat/Synthesis.py` & `foscat-2.0.4/src/foscat/Synthesis.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 from datetime import datetime
 from packaging import version
 from threading import Thread
 from threading import Event
 
 class Loss:
     
-    def __init__(self,function,scat_operator,*param,Rformat=True,name='',batch=None,batch_data=None):
+    def __init__(self,function,scat_operator,*param,
+                 Rformat=True,
+                 name='',
+                 batch=None,
+                 batch_data=None,
+                 batch_update=None):
 
         self.loss_function=function
         self.scat_operator=scat_operator
         self.args=param
         self.Rformat=Rformat
         self.name=name
         self.batch=batch
         self.batch_data=batch_data
+        self.batch_update=batch_update
 
     def eval(self,x,batch):
         if self.batch is None:
             return self.loss_function(x,self.scat_operator,self.args)
         else:
             return self.loss_function(x,batch,self.scat_operator,self.args)
     
@@ -198,16 +204,14 @@
             cur_loss='%.3g ('%(self.ltot[self.ltot!=-1].mean())
             for k in self.ltot[self.ltot!=-1]:
                 cur_loss=cur_loss+'%.3g '%(k)
                 
             cur_loss=cur_loss+')'
                 
             mess=''
-            if self.itt2!=0:
-                mess=' LBFGS %d '%(self.itt2)
                 
             if self.SHOWGPU:
                 info_gpu=self.getgpumem()
                 for k in range(info_gpu.shape[0]):
                     mess=mess+'[GPU%d %.0f/%.0f MB %.0f%%]'%(k,info_gpu[k,0],info_gpu[k,1],info_gpu[k,2])
                 
             print('%sItt %d L=%s %.3fs %s'%(self.MESSAGE,self.itt,cur_loss,(end-self.start),mess))
@@ -228,25 +232,20 @@
             nstep=1
 
         x=self.operation.backend.bk_cast(self.operation.backend.bk_reshape(in_x,self.oshape))
 
         self.l_log[self.mpi_rank*self.MAXNUMLOSS:(self.mpi_rank+1)*self.MAXNUMLOSS]=-1.0
         
         for istep in range(nstep):
-            if self.noise_idx is None:
-                tabidx=((np.arange(self.batchsz)+istep*self.batchsz).astype('int'))%self.totalsz
-            else:
-                tabidx=self.noise_idx
             
-        
             for k in range(self.number_of_loss):
                 if self.loss_class[k].batch is None:
                     l_batch=None
                 else:
-                    l_batch=self.loss_class[k].batch(self.loss_class[k].batch_data,tabidx)
+                    l_batch=self.loss_class[k].batch(self.loss_class[k].batch_data,istep)
 
                 l,g=self.loss(x,l_batch,self.loss_class[k])
 
                 if g_tot is None:
                     g_tot=g
                 else:
                     g_tot=g_tot+g
@@ -301,22 +300,44 @@
         g_tot=grad.flatten()
 
         if g_tot.dtype=='complex64' or g_tot.dtype=='complex128':
             return l_tot.astype('float64'),g_tot
         
         return l_tot.astype('float64'),g_tot.astype('float64')
 
+    # ---------------------------------------------−---------
+    def xtractmap(self,x,axis):
+        x=self.operation.backend.bk_reshape(x,self.oshape)
         
+        operation=self.operation
+        if operation.get_use_R():
+            if axis==0:
+                l_x=operation.to_R(x,only_border=True,chans=self.operation.chans)
+                x=operation.from_R(l_x)
+            else:
+                l_x=operation.to_R(x[0],only_border=True,chans=self.operation.chans)
+                tmp_x=operation.from_R(l_x)
+                out_x=np.zeros([x.shape[0],tmp_x.shape[0]])
+                out_x[0]=tmp_x
+                del tmp_x
+                for i in range(1,self.in_x_nshape):
+                    l_x=operation.to_R(x[i],only_border=True,chans=self.operation.chans)
+                    out_x[i]=operation.from_R(l_x)
+                x=out_x
+        
+        return x
+
     # ---------------------------------------------−---------
     def run(self,
             in_x,
             NUM_EPOCHS = 1000,
             DECAY_RATE=0.95,
             EVAL_FREQUENCY = 100,
             DEVAL_STAT_FREQUENCY = 1000,
+            NUM_STEP_BIAS = 1,
             LEARNING_RATE = 0.03,
             EPSILON = 1E-7,
             grd_mask=None,
             SHOWGPU=False,
             MESSAGE='',
             batchsz=1,
             totalsz=1,
@@ -331,14 +352,15 @@
         self.batchsz=batchsz
         self.totalsz=totalsz
         self.grd_mask=grd_mask
         self.EVAL_FREQUENCY=EVAL_FREQUENCY
         self.MESSAGE=MESSAGE
         self.SHOWGPU=SHOWGPU
         self.axis=axis
+        self.in_x_nshape=in_x.shape[0]
 
         if do_lbfgs and (in_x.dtype=='complex64' or in_x.dtype=='complex128'):
             print('L_BFGS minimisation not yet implemented for acomplex array, use default FOSCAT minimizer or convert your problem to float32 or float64')
             exit(0)
             
         np.random.seed(self.mpi_rank*7+1234)
             
@@ -401,64 +423,67 @@
         self.oshape=list(x.shape)
         
         if not isinstance(x,np.ndarray):
             x=x.numpy()
             
         x=x.flatten()
 
-        self.itt2=0
-        
         self.do_all_noise=False
             
         if do_lbfgs:
             import scipy.optimize as opt
             
             self.do_all_noise=True
 
             self.noise_idx=None
+
+            for k in range(self.number_of_loss):
+                if self.loss_class[k].batch is not None:
+                    l_batch=self.loss_class[k].batch(self.loss_class[k].batch_data,0,init=True)
             
             l_tot,g_tot=self.calc_grad(x)
                 
             self.info_back(x)
 
-            maxitt=NUM_EPOCHS
+            maxitt=NUM_EPOCHS//NUM_STEP_BIAS
 
-            x,l,i=opt.fmin_l_bfgs_b(self.calc_grad,x.astype('float64'),
-                                    callback=self.info_back,
-                                    pgtol=1E-32,
-                                    factr=10.0,
-                                    maxiter=maxitt)
+            start_x=x.copy()
+            
+            for iteration in range(NUM_STEP_BIAS):
+
+                x,l,i=opt.fmin_l_bfgs_b(self.calc_grad,
+                                        x.astype('float64'),
+                                        callback=self.info_back,
+                                        pgtol=1E-32,
+                                        factr=10.0,
+                                        maxiter=maxitt)
+
+                # update bias input data
+                if iteration<NUM_STEP_BIAS-1:
+
+                    omap=self.xtractmap(x,axis)
+
+                    for k in range(self.number_of_loss):
+                        if self.loss_class[k].batch_update is not None:
+                            self.loss_class[k].batch_update(self.loss_class[k].batch_data,omap)
+                            l_batch=self.loss_class[k].batch(self.loss_class[k].batch_data,0,init=True)
+                    #x=start_x.copy()
+                    
         else:
             for itt in range(NUM_EPOCHS):
                 
                 self.noise_idx=((np.random.randn(self.batchsz)*(self.totalsz)+0.49999).astype('int'))%self.totalsz
                 l_tot,g_tot=self.calc_grad(x)
                 
                 x=x-self.update(g_tot)
                 
                 self.info_back(x)
                     
-        x=self.operation.backend.bk_reshape(x,self.oshape)
         
         if self.mpi_rank==0 and SHOWGPU:
             self.stop_synthesis()
-        
-        operation=self.operation
-        if operation.get_use_R():
-            if axis==0:
-                l_x=operation.to_R(x,only_border=True,chans=self.operation.chans)
-                x=operation.from_R(l_x)
-            else:
-                l_x=operation.to_R(x[0],only_border=True,chans=self.operation.chans)
-                tmp_x=operation.from_R(l_x)
-                out_x=np.zeros([x.shape[0],tmp_x.shape[0]])
-                out_x[0]=tmp_x
-                del tmp_x
-                for i in range(1,in_x.shape[0]):
-                    l_x=operation.to_R(x[i],only_border=True,chans=self.operation.chans)
-                    out_x[i]=operation.from_R(l_x)
-                x=out_x
-                    
+
+        x=self.xtractmap(x,axis)
         return(x)
 
     def get_history(self):
         return(self.history[0:self.nlog])
```

### Comparing `foscat-2.0.3/src/foscat/backend.py` & `foscat-2.0.4/src/foscat/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,22 @@
     def bk_log(self,data):
         if self.BACKEND==self.TENSORFLOW:
             return(self.backend.math.log(data))
         if self.BACKEND==self.TORCH:
             return(self.backend.log(data))
         if self.BACKEND==self.NUMPY:
             return(np.log(data))
+
+    def bk_tensor(self,data):
+        if self.BACKEND==self.TENSORFLOW:
+            return(self.backend.constant(data))
+        if self.BACKEND==self.TORCH:
+            return(self.backend.constant(data))
+        if self.BACKEND==self.NUMPY:
+            return(data)
         
     def bk_complex(self,real,imag):
         if self.BACKEND==self.TENSORFLOW:
             return(self.backend.dtypes.complex(real,imag))
         if self.BACKEND==self.TORCH:
             return(self.backend.complex(real,imag))
         if self.BACKEND==self.NUMPY:
```

### Comparing `foscat-2.0.3/src/foscat/build_demo.py` & `foscat-2.0.4/src/foscat/build_demo.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.3/src/foscat/scat.py` & `foscat-2.0.4/src/foscat/scat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 import foscat.FoCUS as FOC
 import numpy as np
 import foscat.Rformat as Rformat
+import tensorflow as tf
 
 def read(filename):
-    thescat=scat(1,1,1,1)
+    thescat=scat(1,1,1,1,1)
     return thescat.read(filename)
     
 class scat:
-    def __init__(self,p00,s0,s1,s2,cross=False,backend=None):
+    def __init__(self,p00,s0,s1,s2,s2l,cross=False,backend=None):
         self.P00=p00
         self.S0=s0
         self.S1=s1
         self.S2=s2
+        self.S2L=s2l
         self.cross=cross
         self.backend=backend
         
+    def get_j_idx(self):
+        shape=list(self.S1.shape)
+        nscale=shape[1]
+        n=nscale*(nscale+1)//2
+        j1=np.zeros([n],dtype='int')
+        j2=np.zeros([n],dtype='int')
+        n=0
+        for i in range(nscale):
+            for j in range(i+1):
+                j1[n]=j
+                j2[n]=i
+                n=n+1
+        return(j1,j2)
+    
     def get_S0(self):
         return(self.S0)
 
     def get_S1(self):
         return(self.S1)
     
     def get_S2(self):
         return(self.S2)
 
+    def get_S2L(self):
+        return(self.S2L)
+
     def get_P00(self):
         return(self.P00)
 
     def reset_P00(self):
         self.P00=0*self.P00
 
     def domult(self,x,y):
@@ -62,123 +81,152 @@
             return x+y
         if x.dtype=='complex64' or x.dtype=='complex128':
             
             return self.backend.bk_complex(self.backend.bk_real(x)+y,self.backend.bk_imag(x)+y)
         else:
             return self.backend.bk_complex(x+self.backend.bk_real(y),x+self.backend.bk_imag(y))
         
+    def relu(self):
+        
+        return scat(self.backend.bk_relu(self.P00), \
+                    self.backend.bk_relu(self.S0), \
+                    self.backend.bk_relu(self.S1), \
+                    self.backend.bk_relu(self.S2), \
+                    self.backend.bk_relu(self.S2L),backend=self.backend)
+
     def __add__(self,other):
         assert isinstance(other, float) or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.doadd(self.P00,other.P00), \
                         self.doadd(self.S0, other.S0), \
                         self.doadd(self.S1, other.S1), \
-                        self.doadd(self.S2, other.S2),backend=self.backend)
+                        self.doadd(self.S2, other.S2), \
+                        self.doadd(self.S2L, other.S2L),backend=self.backend)
         else:
             return scat((self.P00+ other), \
                         (self.S0+ other), \
                         (self.S1+ other), \
-                        (self.S2+ other),backend=self.backend)
+                        (self.S2+ other), \
+                        (self.S2L+ other),backend=self.backend)
 
 
     def __radd__(self,other):
         return self.__add__(other)
 
     def __truediv__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.dodiv(self.P00, other.P00), \
                         self.dodiv(self.S0, other.S0), \
                         self.dodiv(self.S1, other.S1), \
-                        self.dodiv(self.S2, other.S2),backend=self.backend)
+                        self.dodiv(self.S2, other.S2), \
+                        self.dodiv(self.S2L, other.S2L),backend=self.backend)
         else:
             return scat((self.P00/ other), \
                         (self.S0/ other), \
                         (self.S1/ other), \
-                        (self.S2/ other),backend=self.backend)
+                        (self.S2/ other), \
+                        (self.S2L/ other),backend=self.backend)
         
 
     def __rtruediv__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.dodiv(other.P00, self.P00), \
                         self.dodiv(other.S0 , self.S0), \
                         self.dodiv(other.S1 , self.S1), \
-                        self.dodiv(other.S2 , self.S2),backend=self.backend)
+                        self.dodiv(other.S2 , self.S2), \
+                        self.dodiv(other.S2L , self.S2L),backend=self.backend)
         else:
             return scat((other/ self.P00), \
                         (other / self.S0), \
                         (other / self.S1), \
-                        (other / self.S2),backend=self.backend)
+                        (other / self.S2), \
+                        (other / self.S2L),backend=self.backend)
         
     def __sub__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domin(self.P00, other.P00), \
                         self.domin(self.S0, other.S0), \
                         self.domin(self.S1, other.S1), \
-                        self.domin(self.S2, other.S2),backend=self.backend)
+                        self.domin(self.S2, other.S2), \
+                        self.domin(self.S2L, other.S2L),backend=self.backend)
         else:
             return scat((self.P00- other), \
                         (self.S0- other), \
                         (self.S1- other), \
-                        (self.S2- other),backend=self.backend)
+                        (self.S2- other), \
+                        (self.S2L- other),backend=self.backend)
         
     def __rsub__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domin(other.P00,self.P00), \
                         self.domin(other.S0, self.S0), \
                         self.domin(other.S1, self.S1), \
-                        self.domin(other.S2, self.S2),backend=self.backend)
+                        self.domin(other.S2, self.S2), \
+                        self.domin(other.S2L, self.S2L),backend=self.backend)
         else:
             return scat((other-self.P00), \
                         (other-self.S0), \
                         (other-self.S1), \
-                        (other-self.S2),backend=self.backend)
+                        (other-self.S2), \
+                        (other-self.S2L),backend=self.backend)
         
     def __mul__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domult(self.P00, other.P00), \
                         self.domult(self.S0, other.S0), \
                         self.domult(self.S1, other.S1), \
-                        self.domult(self.S2, other.S2),backend=self.backend)
+                        self.domult(self.S2, other.S2), \
+                        self.domult(self.S2L, other.S2L),backend=self.backend)
         else:
             return scat((self.P00* other), \
                         (self.S0* other), \
                         (self.S1* other), \
-                        (self.S2* other),backend=self.backend)
+                        (self.S2* other), \
+                        (self.S2L* other),backend=self.backend)
+    def relu(self):
+        return scat(self.backend.bk_relu(self.P00),
+                    self.backend.bk_relu(self.S0),
+                    self.backend.bk_relu(self.S1),
+                    self.backend.bk_relu(self.S2),
+                    self.backend.bk_relu(self.S2L),backend=self.backend)
+
 
     def __rmul__(self,other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
             isinstance(other, bool) or isinstance(other, scat)
         
         if isinstance(other, scat):
             return scat(self.domult(self.P00, other.P00), \
                         self.domult(self.S0, other.S0), \
                         self.domult(self.S1, other.S1), \
-                        self.domult(self.S2, other.S2),backend=self.backend)
+                        self.domult(self.S2, other.S2), \
+                        self.domult(self.S2L, other.S2L),backend=self.backend)
         else:
             return scat((self.P00* other), \
                         (self.S0* other), \
                         (self.S1* other), \
-                        (self.S2* other),backend=self.backend)
+                        (self.S2* other), \
+                        (self.S2L* other),backend=self.backend)
 
     def l1_abs(self,x):
         y=self.get_np(x)
         if y.dtype=='complex64' or y.dtype=='complex128':
             tmp=y.real*y.real+y.imag*y.imag
             tmp=np.sign(tmp)*np.sqrt(np.fabs(tmp))
             y=tmp
@@ -193,80 +241,206 @@
             name=''
 
         if hold:
             plt.figure(figsize=(8,8))
         
         plt.subplot(2,2,1)
         if legend:
-            plt.plot(abs(self.l1_abs(self.S0).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S0).flatten(),color=color,label=r'%s $S_0$'%(name),lw=lw)
-        else:
-            plt.plot(abs(self.l1_abs(self.S0).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S0).flatten(),color=color,lw=lw)
-        plt.yscale('log')
-        plt.legend()
-        plt.subplot(2,2,2)
-        if legend:
             plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.S1).flatten(),color=color,label=r'%s $S_1$'%(name),lw=lw)
         else:
             plt.plot(abs(self.l1_abs(self.S1).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.S1).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
-        plt.subplot(2,2,3)
+        plt.subplot(2,2,2)
         if legend:
             plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.P00).flatten(),color=color,label=r'%s $P_{00}$'%(name),lw=lw)
         else:
             plt.plot(abs(self.l1_abs(self.P00).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.P00).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
-        plt.subplot(2,2,4)
+        plt.subplot(2,2,3)
         if legend:
             plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
-            plt.plot(self.l1_abs(self.S2).flatten(),color=color,label=r'%s $S_2$'%(name),lw=lw)
+            plt.plot(self.l1_abs(self.S2).flatten(),color=color,label=r'%s $S_2$ L1 norm'%(name),lw=lw)
         else:
             plt.plot(abs(self.l1_abs(self.S2).flatten()),':',color=color,lw=lw)
             plt.plot(self.l1_abs(self.S2).flatten(),color=color,lw=lw)
         plt.yscale('log')
         plt.legend()
         
+        plt.subplot(2,2,4)
+        if legend:
+            plt.plot(abs(self.l1_abs(self.S2L).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S2L).flatten(),color=color,label=r'%s $S_2$ L2 norm'%(name),lw=lw)
+        else:
+            plt.plot(abs(self.l1_abs(self.S2L).flatten()),':',color=color,lw=lw)
+            plt.plot(self.l1_abs(self.S2L).flatten(),color=color,lw=lw)
+        plt.yscale('log')
+        plt.legend()
+        
     def save(self,filename):
         np.save('%s_s0.npy'%(filename), self.get_S0().numpy())
         np.save('%s_s1.npy'%(filename), self.get_S1().numpy())
         np.save('%s_s2.npy'%(filename), self.get_S2().numpy())
+        np.save('%s_s2l.npy'%(filename), self.get_S2L().numpy())
         np.save('%s_p0.npy'%(filename), self.get_P00().numpy())
         
     def read(self,filename):
         s0=np.load('%s_s0.npy'%(filename))
         s1=np.load('%s_s1.npy'%(filename))
         s2=np.load('%s_s2.npy'%(filename))
+        s2l=np.load('%s_s2l.npy'%(filename))
         p0= np.load('%s_p0.npy'%(filename))
-        return scat(p0,s0,s1,s2)
+        return scat(p0,s0,s1,s2,s2l)
     
     def get_np(self,x):
         if isinstance(x, np.ndarray):
             return x
         else:
             return x.numpy()
 
     def std(self):
-        return np.sqrt(((abs(self.get_np(self.S0)).std())**2+(abs(self.get_np(self.S1)).std())**2+(abs(self.get_np(self.S2)).std())**2+(abs(self.get_np(self.P00)).std())**2)/4)
+        return np.sqrt(((abs(self.get_np(self.S0)).std())**2+ \
+                        (abs(self.get_np(self.S1)).std())**2+ \
+                        (abs(self.get_np(self.S2)).std())**2+ \
+                        (abs(self.get_np(self.S2L)).std())**2+ \
+                        (abs(self.get_np(self.P00)).std())**2)/4)
 
     def mean(self):
-        return abs(self.get_np(self.S0).mean()+self.get_np(self.S1).mean()+self.get_np(self.S2).mean()+self.get_np(self.P00).mean())/3
+        return abs(self.get_np(self.S0).mean()+ \
+                   self.get_np(self.S1).mean()+ \
+                   self.get_np(self.S2).mean()+ \
+                   self.get_np(self.S2L).mean()+ \
+                   self.get_np(self.P00).mean())/3
+
+    # ---------------------------------------------−---------
+    def model(self,i__y,add=0,dx=3,dell=2,weigth=None,inverse=False):
+
+        if i__y.shape[0]<dx+1:
+            l__dx=i__y.shape[0]-1
+        else:
+            l__dx=dx
+
+        if i__y.shape[0]<dell:
+            l__dell=0
+        else:
+            l__dell=dell
+
+        if l__dx<2:
+            res=np.zeros([i__y.shape[0]+add])
+            if inverse:
+                res[:-add]=i__y
+            else:
+                res[add:]=i__y[0:]
+            return res
+
+        if weigth is None:
+            w=2**(np.arange(l__dx))
+        else:
+            if not inverse:
+                w=weigth[0:l__dx]
+            else:
+                w=weigth[-l__dx:]
+
+        x=np.arange(l__dx)+1
+        if not inverse:
+            y=np.log(i__y[1:l__dx+1])
+        else:
+            y=np.log(i__y[-(l__dx+1):-1])
+
+        r=np.polyfit(x,y,1,w=w)
+
+        if inverse:
+            res=np.exp(r[0]*(np.arange(i__y.shape[0]+add)-1)+r[1])
+            res[:-(l__dell+add)]=i__y[:-l__dell]
+        else:
+            res=np.exp(r[0]*(np.arange(i__y.shape[0]+add)-add)+r[1])
+            res[l__dell+add:]=i__y[l__dell:]
+        return res
+
+    def findn(self,n):
+        d=np.sqrt(1+8*n)
+        return int((d-1)/2)
+
+    def findidx(self,s2):
+        i1=np.zeros([s2.shape[1]],dtype='int')
+        i2=np.zeros([s2.shape[1]],dtype='int')
+        n=0
+        for k in range(self.findn(s2.shape[1])):
+            i1[n:n+k+1]=np.arange(k+1)
+            i2[n:n+k+1]=k
+            n=n+k+1
+        return i1,i2
+
+    def extrapol_s2(self,add,lnorm=1):
+        if lnorm==1:
+            s2=self.S2.numpy()
+        if lnorm==2:
+            s2=self.S2L.numpy()
+        i1,i2=self.findidx(s2)
+
+        so2=np.zeros([s2.shape[0],(self.findn(s2.shape[1])+add)*(self.findn(s2.shape[1])+add+1)//2,s2.shape[2],s2.shape[3]])
+        oi1,oi2=self.findidx(so2)
+        for l in range(s2.shape[0]):
+            for k in range(self.findn(s2.shape[1])):
+                for i in range(s2.shape[2]):
+                    for j in range(s2.shape[3]):
+                        tmp=self.model(s2[l,i2==k,i,j],dx=4,dell=1,add=add,weigth=np.array([1,2,2,2]))
+                        tmp[np.isnan(tmp)]=0.0
+                        so2[l,oi2==k+add,i,j]=tmp
+
+
+        for l in range(s2.shape[0]):
+            for k in range(add+1,-1,-1):
+                lidx=np.where(oi2-oi1==k)[0]
+                lidx2=np.where(oi2-oi1==k+1)[0]
+                for i in range(s2.shape[2]):
+                    for j in range(s2.shape[3]):
+                        so2[l,lidx[0:add+2-k],i,j]=so2[l,lidx2[0:add+2-k],i,j]
+
+        return(so2)
+
+    def extrapol_s1(self,i_s1,add):
+        s1=i_s1.numpy()
+        so1=np.zeros([s1.shape[0],s1.shape[1]+add,s1.shape[2]])
+        for k in range(s1.shape[0]):
+            for i in range(s1.shape[2]):
+                so1[k,:,i]=self.model(s1[k,:,i],dx=4,dell=1,add=add)
+                so1[k,np.isnan(so1[k,:,i]),i]=0.0
+        return so1
+
+    def extrapol(self,add):
+        return scat(self.extrapol_s1(self.P00,add), \
+                    self.S0, \
+                    self.extrapol_s1(self.S1,add), \
+                    self.extrapol_s2(add,lnorm=1), \
+                    self.extrapol_s2(add,lnorm=2),backend=self.backend)
+        
+        
         
         
     
 class funct(FOC.FoCUS):
     
     def eval(self, image1, image2=None,mask=None,Auto=True,s0_off=1E-6):
-
+        # Check input consistency
+        if not isinstance(image1,Rformat.Rformat):
+            if image2 is not None:
+                if list(image1.shape)!=list(image2.shape):
+                    print('The two input image should have the same size to eval Scattering')
+                    exit(0)
+            if mask is not None:
+                if list(image1.shape)!=list(mask.shape)[1:]:
+                    print('The mask should have the same size than the input image to eval Scattering')
+                    exit(0)
+            
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=not Auto
         else:
             all_cross=False
@@ -335,15 +509,14 @@
             if cross:
                 l_image2=self.up_grade(I2,nside*2,axis=axis)
         else:
             l_image1=I1
             if cross:
                 l_image2=I2
 
-        s0=None
         s0 = self.masked_mean(l_image1,vmask,axis=axis)+s0_off
         
         if cross and Auto==False:
             if len(image1.shape)==1 or (len(image1.shape)==3 and isinstance(image1,Rformat.Rformat)):
                 if s0.dtype!='complex64' and s0.dtype!='complex128':
                     s0 = self.backend.bk_complex(s0,self.masked_mean(l_image2,vmask,axis=axis)+s0_off)
                 else:
@@ -352,14 +525,15 @@
                 if s0.dtype!='complex64' and s0.dtype!='complex128':
                     s0 = self.backend.bk_complex(s0,self.masked_mean(l_image2,vmask,axis=axis)+s0_off)
                 else:
                     s0 = self.backend.bk_concat([s0,self.masked_mean(l_image2,vmask,axis=axis)],axis=0)
 
         s1=None
         s2=None
+        s2l=None
         p00=None
         l2_image=None
         l2_image_imag=None
 
         for j1 in range(jmax):
             # Convol image along the axis defined by 'axis' using the wavelet defined at
             # the foscat initialisation
@@ -397,32 +571,41 @@
                 l2_image=self.backend.bk_expand_dims(self.update_R_border(conj,axis=axis),axis=-2)
             else:
                 l2_image=self.backend.bk_concat([self.backend.bk_expand_dims(self.update_R_border(conj,axis=axis),axis=-2),l2_image],axis=-2)
 
             # Convol l2_image [....,Npix_j1,....,j1,Norient,Norient]
             c2_image=self.convol(self.backend.bk_relu(l2_image),axis=axis)
 
-            conj2p=self.backend.bk_L1(c2_image*self.backend.bk_conjugate(c2_image))
+            conj2p=c2_image*self.backend.bk_conjugate(c2_image)
+            conj2pl1=self.backend.bk_L1(conj2p)
+
             if Auto:
                 conj2p=self.backend.bk_real(conj2p)
+                conj2pl1=self.backend.bk_real(conj2pl1)
 
             c2_image=self.convol(self.backend.bk_relu(-l2_image),axis=axis)
 
-            conj2m=self.backend.bk_L1(c2_image*self.backend.bk_conjugate(c2_image))
+            conj2m=c2_image*self.backend.bk_conjugate(c2_image)
+            conj2ml1=self.backend.bk_L1(conj2m)
+
             if Auto:
                 conj2m=self.backend.bk_real(conj2m)
+                conj2ml1=self.backend.bk_real(conj2ml1)
 
             # Convol l_s2 [....,....,Nmask,j1,Norient,Norient]
             l_s2 = self.masked_mean(conj2p-conj2m,vmask,axis=axis)
+            l_s2l1 = self.masked_mean(conj2pl1-conj2ml1,vmask,axis=axis)
 
             # Concat l_s2 [....,....,Nmask,j1*(j1+1)/2,Norient,Norient]
             if s2 is None:
-                s2=l_s2
+                s2l=l_s2
+                s2=l_s2l1
             else:
-                s2=self.backend.bk_concat([s2,l_s2],axis=-3)
+                s2=self.backend.bk_concat([s2,l_s2l1],axis=-3)
+                s2l=self.backend.bk_concat([s2l,l_s2],axis=-3)
 
             if j1!=jmax-1:
                 # Rescale vmask [Nmask,Npix_j1//4]   
                 vmask = self.smooth(vmask,axis=1)
                 vmask = self.ud_grade_2(vmask,axis=1)
 
                 # Rescale l2_image [....,Npix_j1//4,....,j1,Norient]   
@@ -433,85 +616,107 @@
                 l_image1 = self.smooth(l_image1,axis=axis)
                 l_image1 = self.ud_grade_2(l_image1,axis=axis)
                 if cross:
                     l_image2 = self.smooth(l_image2,axis=axis)
                     l_image2 = self.ud_grade_2(l_image2,axis=axis)
                     
         if len(image1.shape)==1 or (len(image1.shape)==3 and isinstance(image1,Rformat.Rformat)):
-            return(scat(p00[0],s0[0],s1[0],s2[0],cross,backend=self.backend))
+            return(scat(p00[0],s0[0],s1[0],s2[0],s2l[0],cross,backend=self.backend))
 
-        return(scat(p00,s0,s1,s2,cross,backend=self.backend))
+        return(scat(p00,s0,s1,s2,s2l,cross,backend=self.backend))
 
     def square(self,x):
         # the abs make the complex value usable for reduce_sum or mean
         return scat(self.backend.bk_square(self.backend.bk_abs(x.P00)),
                     self.backend.bk_square(self.backend.bk_abs(x.S0)),
                     self.backend.bk_square(self.backend.bk_abs(x.S1)),
-                    self.backend.bk_square(self.backend.bk_abs(x.S2)),backend=self.backend)
+                    self.backend.bk_square(self.backend.bk_abs(x.S2)),
+                    self.backend.bk_square(self.backend.bk_abs(x.S2L)),backend=self.backend)
     
     def sqrt(self,x):
         # the abs make the complex value usable for reduce_sum or mean
         return scat(self.backend.bk_sqrt(self.backend.bk_abs(x.P00)),
                     self.backend.bk_sqrt(self.backend.bk_abs(x.S0)),
                     self.backend.bk_sqrt(self.backend.bk_abs(x.S1)),
-                    self.backend.bk_sqrt(self.backend.bk_abs(x.S2)),backend=self.backend)
+                    self.backend.bk_sqrt(self.backend.bk_abs(x.S2)),
+                    self.backend.bk_sqrt(self.backend.bk_abs(x.S2L)),backend=self.backend)
 
     def reduce_mean(self,x,axis=None):
         if axis is None:
             tmp=self.backend.bk_abs(self.backend.bk_reduce_sum(x.P00))+ \
                  self.backend.bk_abs(self.backend.bk_reduce_sum(x.S0))+ \
                  self.backend.bk_abs(self.backend.bk_reduce_sum(x.S1))+ \
-                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2))
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2L))
             
             ntmp=np.array(list(x.P00.shape)).prod()+ \
                   np.array(list(x.S0.shape)).prod()+ \
                   np.array(list(x.S1.shape)).prod()+ \
                   np.array(list(x.S2.shape)).prod()
             
             return  tmp/ntmp
         else:
             tmp=self.backend.bk_abs(self.backend.bk_reduce_sum(x.P00,axis=axis))+ \
                  self.backend.bk_abs(self.backend.bk_reduce_sum(x.S0,axis=axis))+ \
                  self.backend.bk_abs(self.backend.bk_reduce_sum(x.S1,axis=axis))+ \
-                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2,axis=axis))
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2,axis=axis))+ \
+                 self.backend.bk_abs(self.backend.bk_reduce_sum(x.S2L,axis=axis))
             
             ntmp=np.array(list(x.P00.shape)).prod()+ \
                   np.array(list(x.S0.shape)).prod()+ \
                   np.array(list(x.S1.shape)).prod()+ \
-                  np.array(list(x.S2.shape)).prod()
+                  np.array(list(x.S2.shape)).prod()+ \
+                  np.array(list(x.S2L.shape)).prod()
             
             return  tmp/ntmp
 
     def reduce_sum(self,x,axis=None):
         if axis is None:
             return  self.backend.bk_reduce_sum(self.backend.bk_abs(x.P00))+ \
                 self.backend.bk_reduce_sum(self.backend.bk_abs(x.S0))+ \
                 self.backend.bk_reduce_sum(self.backend.bk_abs(x.S1))+ \
-                self.backend.bk_reduce_sum(self.backend.bk_abs(x.S2))
+                self.backend.bk_reduce_sum(self.backend.bk_abs(x.S2))+ \
+                self.backend.bk_reduce_sum(self.backend.bk_abs(x.S2L))
         else:
             return scat(self.backend.bk_reduce_sum(x.P00,axis=axis),
                         self.backend.bk_reduce_sum(x.S0,axis=axis),
                         self.backend.bk_reduce_sum(x.S1,axis=axis),
-                        self.backend.bk_reduce_sum(x.S2,axis=axis),backend=self.backend)
+                        self.backend.bk_reduce_sum(x.S2,axis=axis),
+                        self.backend.bk_reduce_sum(x.S2L,axis=axis),backend=self.backend)
         
     def ldiff(self,sig,x):
         return scat(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
                     x.domult(sig.S0,x.S0)*x.domult(sig.S0,x.S0),
                     x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
-                    x.domult(sig.S2,x.S2)*x.domult(sig.S2,x.S2),backend=self.backend)
+                    x.domult(sig.S2,x.S2)*x.domult(sig.S2,x.S2),
+                    x.domult(sig.S2L,x.S2L)*x.domult(sig.S2L,x.S2L),backend=self.backend)
 
     def log(self,x):
         return scat(self.backend.bk_log(x.P00),
                     self.backend.bk_log(x.S0),
                     self.backend.bk_log(x.S1),
-                    self.backend.bk_log(x.S2),backend=self.backend)
+                    self.backend.bk_log(x.S2),
+                    self.backend.bk_log(x.S2L),backend=self.backend)
     def abs(self,x):
         return scat(self.backend.bk_abs(x.P00),
                     self.backend.bk_abs(x.S0),
                     self.backend.bk_abs(x.S1),
-                    self.backend.bk_abs(x.S2),backend=self.backend)
+                    self.backend.bk_abs(x.S2),
+                    self.backend.bk_abs(x.S2L),backend=self.backend)
     def inv(self,x):
-        return scat(1/(x.P00),1/(x.S0),1/(x.S1),1/(x.S2),backend=self.backend)
+        return scat(1/(x.P00),1/(x.S0),1/(x.S1),1/(x.S2),1/(x.S2L),backend=self.backend)
 
     def one(self):
-        return scat(1.0,1.0,1.0,1.0,backend=self.backend)
+        return scat(1.0,1.0,1.0,1.0,1.0,backend=self.backend)
+
+    @tf.function
+    def eval_comp_fast(self, image1, image2=None,mask=None,Auto=True,s0_off=1E-6):
+
+        res=self.eval(image1, image2=image2,mask=mask,Auto=Auto,s0_off=s0_off)
+        return res.P00,res.S0,res.S1,res.S2,res.S2L
+
+    def eval_fast(self, image1, image2=None,mask=None,Auto=True,s0_off=1E-6):
+        p0,s0,s1,s2,s2l=self.eval_comp_fast(image1, image2=image2,mask=mask,Auto=Auto,s0_off=s0_off)
+        return scat(p0,s0,s1,s2,s2l,backend=self.backend)
+        
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `foscat-2.0.3/src/foscat/scat_cov.old.py` & `foscat-2.0.4/src/foscat/scat_cov.old.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.3/src/foscat/scat_cov.py` & `foscat-2.0.4/src/foscat/scat_cov.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,28 @@
 
     def get_C10(self):
         return self.C10
 
     def get_C11(self):
         return self.C11
 
+    def get_j_idx(self):
+        shape=list(self.P00.shape)
+        nscale=shape[2]
+        n=nscale*(nscale-1)//2
+        j1=np.zeros([n],dtype='int')
+        j2=np.zeros([n],dtype='int')
+        n=0
+        for i in range(nscale):
+            for j in range(i):
+                j1[n]=j
+                j2[n]=i
+                n=n+1
+        return(j1,j2)
+    
     def __add__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
         if self.S1 is None:
             s1 = None
         else:
@@ -95,14 +109,39 @@
                             (self.C01 + other.C01),
                             c11,s1=s1, c10=c10,backend=self.backend)
         else:
             return scat_cov((self.P00 + other),
                             (self.C01 + other),
                             c11,s1=s1, c10=c10,backend=self.backend)
 
+    
+    def relu(self):
+
+        if self.S1 is None:
+            s1 = None
+        else:
+            s1 = self.backend.bk_relu(self.S1)
+
+        if self.C10 is None:
+            c10 = None
+        else:
+            c10 = self.backend.bk_relu(self.c10)
+                
+        if self.C11 is None:
+            c11 = None
+        else:
+            c11 = self.backend.bk_relu(self.c11)
+
+        return scat_cov(self.backend.bk_relu(self.P00),
+                        self.backend.bk_relu(self.C01),
+                        c11,
+                        s1=s1, 
+                        c10=c10,
+                        backend=self.backend)
+
     def __radd__(self, other):
         return self.__add__(other)
     
     def __truediv__(self, other):
         assert isinstance(other, float)  or isinstance(other, np.float32) or isinstance(other, int) or \
                isinstance(other, bool) or isinstance(other, scat_cov)
 
@@ -683,14 +722,25 @@
         all_cross: False or True
             If False compute all the coefficient even the Imaginary part,
             If True return only the terms computable in the auto case.
         Returns
         -------
         S1, P00, C01, C11 normalized
         """
+        # Check input consistency
+        if not isinstance(image1,Rformat.Rformat):
+            if image2 is not None:
+                if list(image1.shape)!=list(image2.shape):
+                    print('The two input image should have the same size to eval Scattering')
+                    exit(0)
+            if mask is not None:
+                if list(image1.shape)!=list(mask.shape)[1:]:
+                    print('The mask should have the same size than the input image to eval Scattering')
+                    exit(0)
+
         ### AUTO OR CROSS
         cross = False
         if image2 is not None:
             cross = True
             all_cross=Auto
         else:
             all_cross=False
@@ -1104,26 +1154,39 @@
         else:
             return self.backend.bk_reduce_sum(x)
         return result
 
         
     def ldiff(self,sig,x):
 
-                
         if x.S1 is None:
-            return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
-                            x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
-                            x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
-                            backend=self.backend)
-        else:
-            return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
-                            x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
-                            x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
-                            x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
-                            backend=self.backend)
+            if x.C11 is not None:
+                return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                                x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                                x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
+                                backend=self.backend)
+            else:
+                return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                                x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                                0*sig.C01,
+                                backend=self.backend)
+        else:
+            if x.C11 is None:
+                return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                                x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
+                                x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                                0*sig.S1,
+                                backend=self.backend)
+            else:
+                return scat_cov(x.domult(sig.P00,x.P00)*x.domult(sig.P00,x.P00),
+                                x.domult(sig.S1,x.S1)*x.domult(sig.S1,x.S1),
+                                x.domult(sig.C01,x.C01)*x.domult(sig.C01,x.C01),
+                                x.domult(sig.C11,x.C11)*x.domult(sig.C11,x.C11),
+                                backend=self.backend)
+
     
     def log(self, x):
         if isinstance(x, scat_cov):
 
             if x.S1 is None:
                 result = self.backend.bk_log(x.P00) + \
                          self.backend.bk_log(x.C01) + \
```

### Comparing `foscat-2.0.3/src/foscat/scat_cov_new.py` & `foscat-2.0.4/src/foscat/scat_cov_new.py`

 * *Files identical despite different names*

### Comparing `foscat-2.0.3/src/foscat.egg-info/PKG-INFO` & `foscat-2.0.4/src/foscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foscat
-Version: 2.0.3
+Version: 2.0.4
 Summary: Generate synthetic Healpix or 2D data using Cross Scattering Transform
 Home-page: https://github.com/jmdelouis/FOSCAT
 Author: Jean-Marc DELOUIS
 Author-email: jean.marc.delouis@ifremer.fr
 Maintainer: Theo Foulquier
 Maintainer-email: theo.foulquier@ifremer.fr
 License: MIT
```

