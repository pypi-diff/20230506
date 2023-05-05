# Comparing `tmp/VAE_G2P-0.0.9.tar.gz` & `tmp/VAE_G2P-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VAE_G2P-0.0.9.tar", last modified: Thu Apr 27 19:25:47 2023, max compression
+gzip compressed data, was "VAE_G2P-0.1.0.tar", last modified: Fri May  5 22:05:56 2023, max compression
```

## Comparing `VAE_G2P-0.0.9.tar` & `VAE_G2P-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.239858 VAE_G2P-0.0.9/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 19:25:47.239647 VAE_G2P-0.0.9/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.0.9/README.md
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.238667 VAE_G2P-0.0.9/VAE_G2P/
--rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.0.9/VAE_G2P/__init__.py
--rw-r--r--   0 davidblair   (501) staff       (20)    19656 2023-04-27 19:24:00.000000 VAE_G2P-0.0.9/VAE_G2P/basic_g2p.py
--rw-r--r--   0 davidblair   (501) staff       (20)    13488 2023-04-05 04:47:18.000000 VAE_G2P-0.0.9/VAE_G2P/cvae_model.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15935 2023-04-27 17:27:13.000000 VAE_G2P-0.0.9/VAE_G2P/data.py
--rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.0.9/VAE_G2P/data_wrapper.py
--rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.0.9/VAE_G2P/networks.py
--rw-r--r--   0 davidblair   (501) staff       (20)    15046 2023-04-05 04:47:50.000000 VAE_G2P-0.0.9/VAE_G2P/optim.py
--rw-r--r--   0 davidblair   (501) staff       (20)    23311 2023-04-27 19:24:46.000000 VAE_G2P-0.0.9/VAE_G2P/vae_g2p.py
-drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-04-27 19:25:47.239373 VAE_G2P-0.0.9/VAE_G2P.egg-info/
--rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/PKG-INFO
--rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/SOURCES.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/dependency_links.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/requires.txt
--rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-04-27 19:25:47.000000 VAE_G2P-0.0.9/VAE_G2P.egg-info/top_level.txt
--rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-04-27 19:25:47.239897 VAE_G2P-0.0.9/setup.cfg
--rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.0.9/setup.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-05-05 22:05:56.486071 VAE_G2P-0.1.0/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-05-05 22:05:56.485924 VAE_G2P-0.1.0/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      158 2023-03-05 01:23:50.000000 VAE_G2P-0.1.0/README.md
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-05-05 22:05:56.484823 VAE_G2P-0.1.0/VAE_G2P/
+-rw-r--r--   0 davidblair   (501) staff       (20)      130 2023-04-05 04:44:26.000000 VAE_G2P-0.1.0/VAE_G2P/__init__.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    19824 2023-05-05 21:52:09.000000 VAE_G2P-0.1.0/VAE_G2P/basic_g2p.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    14796 2023-05-05 22:01:52.000000 VAE_G2P-0.1.0/VAE_G2P/cvae_model.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    16086 2023-05-02 19:02:42.000000 VAE_G2P-0.1.0/VAE_G2P/data.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     2120 2023-03-30 02:16:44.000000 VAE_G2P-0.1.0/VAE_G2P/data_wrapper.py
+-rw-r--r--   0 davidblair   (501) staff       (20)     9624 2023-03-08 05:48:31.000000 VAE_G2P-0.1.0/VAE_G2P/networks.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    15646 2023-05-05 17:44:58.000000 VAE_G2P-0.1.0/VAE_G2P/optim.py
+-rw-r--r--   0 davidblair   (501) staff       (20)    23320 2023-05-05 21:53:31.000000 VAE_G2P-0.1.0/VAE_G2P/vae_g2p.py
+drwxr-xr-x   0 davidblair   (501) staff       (20)        0 2023-05-05 22:05:56.485719 VAE_G2P-0.1.0/VAE_G2P.egg-info/
+-rw-r--r--   0 davidblair   (501) staff       (20)      486 2023-05-05 22:05:56.000000 VAE_G2P-0.1.0/VAE_G2P.egg-info/PKG-INFO
+-rw-r--r--   0 davidblair   (501) staff       (20)      331 2023-05-05 22:05:56.000000 VAE_G2P-0.1.0/VAE_G2P.egg-info/SOURCES.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        1 2023-05-05 22:05:56.000000 VAE_G2P-0.1.0/VAE_G2P.egg-info/dependency_links.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       34 2023-05-05 22:05:56.000000 VAE_G2P-0.1.0/VAE_G2P.egg-info/requires.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)        8 2023-05-05 22:05:56.000000 VAE_G2P-0.1.0/VAE_G2P.egg-info/top_level.txt
+-rw-r--r--   0 davidblair   (501) staff       (20)       38 2023-05-05 22:05:56.486120 VAE_G2P-0.1.0/setup.cfg
+-rw-r--r--   0 davidblair   (501) staff       (20)      941 2023-04-05 04:37:12.000000 VAE_G2P-0.1.0/setup.py
```

### Comparing `VAE_G2P-0.0.9/VAE_G2P/basic_g2p.py` & `VAE_G2P-0.1.0/VAE_G2P/basic_g2p.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
             freq_loss=dist.OrderedLogistic(freq_logits[freq_obs_mask],cut_points).log_prob(obs_freq_classes[freq_obs_mask]).sum()
         else:
             freq_loss=0.0
 
         return -1.0*(symptom_annot_loss+missing_loss+freq_loss)
 
 
-class BasicG2PMapLoss_Categortical(nn.Module):
+class BasicG2PMapLoss_Categorical(nn.Module):
     def __init__(self):
-        super(BasicG2PMapLoss_Categortical,self).__init__()
+        super(BasicG2PMapLoss_Categorical,self).__init__()
 
     def forward(self,symptoms_logits,missing_logits, freq_logits, obs_symptoms, obs_freq_classes):
         symptom_annot_loss=dist.Bernoulli(logits=symptoms_logits).log_prob(obs_symptoms).sum()
 
         freq_missing=torch.zeros(obs_freq_classes.shape,dtype=torch.float32,device=freq_logits.device)
         freq_missing[(obs_freq_classes==-1.0)]=1.0
         missing_loss=dist.Bernoulli(logits=missing_logits[obs_symptoms==1.0]).log_prob(freq_missing[obs_symptoms==1.0]).sum()
@@ -153,14 +153,17 @@
         cut_points=[0.04,0.3,0.8,0.99]
         ):
         self.g2p_dataset=g2p_dataset
         self.cut_points=torch.logit(torch.tensor(cut_points,dtype=torch.float32))
 
         self.n_pred=len(self.g2p_dataset.symptom_map)
         self.n_freq_class=len(self.g2p_dataset.ordinal_freq_map)-1
+        if g2p_dataset.aux_gene_info_table['return_dim'].sum()==0:
+            raise ValueError("Gene-specific features are required in order to fit the BasicG2PModel.")
+
         self.basic_net = BasicG2PMap(self.g2p_dataset.aux_gene_info_table['return_dim'].sum(), self.n_pred,self.n_freq_class,network_hyperparameters=network_hyperparameters)
         self.basic_net.eval()
 
     def Fit(self,batch_size,learning_rate,max_epochs,errorTol,compute_device=None,numDataLoaders=0,verbose=True,logFile=None,early_stop_patience=5,monitor_validation=False,weight_decay=0.0001):
 
         if compute_device is None:
             compute_device='cpu'
@@ -388,15 +391,15 @@
 
         pred_log_odds=self.basic_net.forward(data_arrays[2])
         if in_training:
             self.basic_net.train()
 
         null_model_log_odds=tuple(torch.logit(self.g2p_dataset._torchWrapper(x)).unsqueeze(dim=0) for x in self.g2p_dataset.InferNullModel().values())
         output=np.zeros((pred_log_odds[0].shape[0],3))
-        perplex_function_null=BasicG2PMapLoss_Categortical()
+        perplex_function_null=BasicG2PMapLoss_Categorical()
         perplex_function_basic=BasicG2PMapLoss()
         for i in range(output.shape[0]):
             output[i,0]=perplex_function_basic(pred_log_odds[0][i:i+1],pred_log_odds[1][i:i+1],pred_log_odds[2][i:i+1], data_arrays[0][i:i+1],data_arrays[1][i:i+1],self.cut_points).detach().item()
             output[i,1]=perplex_function_null(null_model_log_odds[0],null_model_log_odds[1],null_model_log_odds[2], data_arrays[0][i:i+1],data_arrays[1][i:i+1]).detach().item()
             output[i,2]=output[i,0]-output[i,1]
 
         return {'BasicG2PModel Perplex.':output[:,0],'Null Perplex.':output[:,1],'BasicG2PModel-Null':output[:,2]}
```

### Comparing `VAE_G2P-0.0.9/VAE_G2P/cvae_model.py` & `VAE_G2P-0.1.0/VAE_G2P/cvae_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import copy
 from pyro.infer import Trace_ELBO
 
 from .networks import FC_MeanScaleEncoder,FC_Decoder,Linear_Decoder
 
 class DiseaseCondVAE(nn.Module):
 
+
 	def __init__(self,
 		num_symptoms,
 		n_freq_classes,
 		n_latent_dim,
-		baseline_g2p_model,
+		baseline_g2p_model=None,
 		isLinear=True,
 		encoder_hyperparameters={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True},
 		decoder_hyperparameters={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True},
 		missing_freq_prior_mean=0.0,
 		missing_freq_prior_scale=3.0,
 		cut_points = [0.04,0.3,0.8,0.99]
 		):    
@@ -26,16 +27,20 @@
 		self.num_symptoms=num_symptoms
 		self.n_latent_dim=n_latent_dim
 		self.n_freq_classes=n_freq_classes
 		self.baseline_g2p_model=baseline_g2p_model
 
 
 		#encoder receives the following information: annotated symptoms, whether frequency is present or missing, and the assigned frequency. This information can be encoded using self.num_dx (annotation present)+self.num_dx (frequency present vs missing)+ self.num_dx*(self.n_freq_classes) (using one-hot endoding)
-		self.encoder=FC_MeanScaleEncoder((self.n_freq_classes+2)*self.num_symptoms+self.baseline_g2p_model.g2p_dataset.aux_gene_info_table['return_dim'].sum(),n_latent_dim,**encoder_hyperparameters)
-		self.prior_model=FC_MeanScaleEncoder(3*self.num_symptoms+self.baseline_g2p_model.g2p_dataset.aux_gene_info_table['return_dim'].sum(),n_latent_dim,**encoder_hyperparameters)
+		if self.baseline_g2p_model is not None:
+			self.encoder=FC_MeanScaleEncoder((self.n_freq_classes+2)*self.num_symptoms+self.baseline_g2p_model.g2p_dataset.aux_gene_info_table['return_dim'].sum(),n_latent_dim,**encoder_hyperparameters)
+			self.prior_model=FC_MeanScaleEncoder((self.n_freq_classes+2)*self.num_symptoms+self.baseline_g2p_model.g2p_dataset.aux_gene_info_table['return_dim'].sum(),n_latent_dim,**encoder_hyperparameters)
+		else:
+			self.encoder=FC_MeanScaleEncoder((self.n_freq_classes+2)*self.num_symptoms,n_latent_dim,**encoder_hyperparameters)
+			self.prior_model=None
 
 		self.isLinear=isLinear
 
 		if self.isLinear:
 			self.symptom_annotation_decoder=Linear_Decoder(n_latent_dim,self.num_symptoms)
 			self.symptom_frequency_decoder=Linear_Decoder(n_latent_dim,self.num_symptoms)
 		else:
@@ -56,14 +61,16 @@
 		self.missing_freq_intercepts_post_mean=torch.zeros(self.num_symptoms,dtype=torch.float32)
 		self.missing_freq_intercepts_post_log_scale=torch.zeros(self.num_symptoms,dtype=torch.float32)
 
 		
 		self.compute_device='cpu'
 		self.eval()
 
+
+
 	def model(self,annot_data=None,freq_data=None,gene_data=None,num_samples=None,minibatch_scale=1.0, annealing_factor=1.0):
 		if annot_data is not None:
 			num_samples=annot_data.shape[0]
 		else:
 			if num_samples is None:
 				num_samples=1000
 				print('Warning: no arguments were given to DiseaseVAE.model. This should only be done during debugging.')
@@ -87,32 +94,41 @@
 			transformed_freq_data=None
 
 
 
 		pyro.module("symptom_annotation_decoder", self.symptom_annotation_decoder)
 		pyro.module("symptom_frequency_decoder", self.symptom_frequency_decoder)
 		pyro.module("missing_freq_disease_decoder", self.missing_freq_disease_decoder)
-		pyro.module("prior_model",self.prior_model)
+		if self.prior_model is not None:
+			pyro.module("prior_model",self.prior_model)
 
 		with torch.no_grad():
 			self.missing_freq_prior_scale=self.missing_freq_prior_scale.detach().to(self.compute_device)
 			self.missing_freq_prior_mean=self.missing_freq_prior_mean.detach().to(self.compute_device)
 			self.cut_points=self.cut_points.detach().to(self.compute_device)
 
 		self.missing_freq_intercepts=pyro.sample("missing_freq_intercepts", dist.Normal(torch.zeros(self.num_symptoms,dtype=torch.float32,device=self.compute_device)+self.missing_freq_prior_mean, torch.ones(self.num_symptoms,dtype=torch.float32,device=self.compute_device)*self.missing_freq_prior_scale).to_event(1))
 
 
 		with pyro.poutine.scale(None,minibatch_scale):
 
 			with pyro.plate("data",size=num_samples,dim=-2):
-				with torch.no_grad():
-					gene_pred= self.baseline_g2p_model.basic_net.forward(gene_data)
-					gene_pred=torch.cat(gene_pred,axis=1)
-				z_loc,z_scale = self.prior_model(torch.cat((gene_pred,gene_data),axis=1))
+				if self.prior_model is not None: 
+					with torch.no_grad():
+						gene_pred= self.baseline_g2p_model.basic_net.forward(gene_data)
+						annot_hat=torch.sigmoid(gene_pred[0])
+						missing_hat=torch.sigmoid(gene_pred[1])
+						freq_hat=torch.exp(dist.OrderedLogistic(gene_pred[2],self.cut_points).logits).flatten(start_dim=1)
+						disease_info_hat=torch.cat([annot_hat,missing_hat,freq_hat],axis=1)
+					z_loc,z_scale = self.prior_model(torch.cat((disease_info_hat,gene_data),axis=1))
+				else:
+					z_loc = torch.zeros(torch.Size((num_samples, self.n_latent_dim)),dtype=torch.float32,device=self.compute_device)
+					z_scale = torch.ones(torch.Size((num_samples, self.n_latent_dim)),dtype=torch.float32,device=self.compute_device)
 				with pyro.poutine.scale(None, annealing_factor):
+
 					latent_variables=pyro.sample("latent_variables",dist.Normal(z_loc,z_scale))
 
 
 				annotation_pred = self.symptom_annotation_decoder.forward(latent_variables)
 				annotation_outcomes = pyro.sample("annotation_outcomes",dist.Bernoulli(logits=annotation_pred),obs=annot_data)
 
 
@@ -180,16 +196,18 @@
 			#assign unnannotated and missing data to an unobserved class
 			transformed_freq_data=freq_data.detach().clone().long()
 
 			transformed_freq_data[freq_data==-1]=len(self.cut_points)+1
 			transformed_freq_data[(annot_data==0)]=len(self.cut_points)+1
 
 			unrolled_freq_classes = torch.nn.functional.one_hot(transformed_freq_data)
-
-			input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1),gene_data],axis=1)
+			if gene_data is not None:
+				input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1),gene_data],axis=1)
+			else:
+				input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1)],axis=1)
 			z_mean,z_std = self.encoder.forward(input_data)
 			with pyro.poutine.scale(None, annealing_factor):
 				with pyro.plate("data",size=num_samples,dim=-2):
 					pyro.sample("latent_variables", dist.Normal(z_mean, z_std))
 
 	def posterior_latent_state(self,annot_data,freq_data,gene_data):
 		if self.training:
@@ -204,16 +222,18 @@
 		#assign unnannotated and missing data to an unobserved class
 		transformed_freq_data=freq_data.detach().clone().long()
 
 		transformed_freq_data[freq_data==-1]=len(self.cut_points)+1
 		transformed_freq_data[(annot_data==0)]=len(self.cut_points)+1
 
 		unrolled_freq_classes = torch.nn.functional.one_hot(transformed_freq_data)
-
-		input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1),gene_data],axis=1)
+		if gene_data is not None:
+			input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1),gene_data],axis=1)
+		else:
+			input_data=torch.cat([annot_data,missing_freqs,unrolled_freq_classes[:,:,:-1].flatten(start_dim=1)],axis=1)
 
 
 		p_mean,p_std=self.encoder.forward(input_data)
 		if in_training:
 			self.train()
 
 		return p_mean.detach(),p_std.detach()
@@ -226,19 +246,22 @@
 		-------
 		dict
 		    Model state dict.
 
 		"""
 		packaged_model_state={}
 		packaged_model_state['model_state'] = copy.deepcopy(self.state_dict(keep_vars=True))
-		packaged_model_state['baseline_g2p_model'] = copy.deepcopy(self.baseline_g2p_model.basic_net.state_dict(keep_vars=True))
+		
 		packaged_model_state['variational_post_params']={}
 		packaged_model_state['variational_post_params']['missing_freq_intercepts_post_mean']=self.missing_freq_intercepts_post_mean.detach()
 		packaged_model_state['variational_post_params']['missing_freq_intercepts_post_log_scale']=self.missing_freq_intercepts_post_log_scale.detach()
-		
+		if self.baseline_g2p_model is not None:
+			packaged_model_state['baseline_g2p_model'] = copy.deepcopy(self.baseline_g2p_model.basic_net.state_dict(keep_vars=True))
+		else:
+			packaged_model_state['baseline_g2p_model']=None
 		return packaged_model_state
 
 	def load_state(self,prior_model_state):
 		"""
 		Loads model state from dictionary
 
 		Parameters
@@ -248,31 +271,35 @@
 
 		Returns
 		-------
 		None
 
 		"""
 		self.load_state_dict(prior_model_state['model_state'],strict=True)
-		self.baseline_g2p_model.basic_net.load_state_dict(prior_model_state['baseline_g2p_model'],strict=True)
 		self.missing_freq_intercepts_post_mean=prior_model_state['variational_post_params']['missing_freq_intercepts_post_mean']
 		self.missing_freq_intercepts_post_log_scale=prior_model_state['variational_post_params']['missing_freq_intercepts_post_log_scale']
+		if self.baseline_g2p_model is not None:
+			self.baseline_g2p_model.basic_net.load_state_dict(prior_model_state['baseline_g2p_model'],strict=True)
+		else:
+			self.baseline_g2p_model=None
 
 	def switch_device(self, new_compute_device):
 		"""Sw
 
 		Parameters
 		----------
 		compute_device : str
 		    String name for compute device. Ideally expressed as 'type:number'
 		"""
 		self.compute_device=new_compute_device
 		self.to(self.compute_device)
 		self.missing_freq_intercepts_post_mean.to(self.compute_device)
 		self.missing_freq_intercepts_post_log_scale.to(self.compute_device)
-		self.baseline_g2p_model.basic_net.to(self.compute_device)
+		if self.baseline_g2p_model is not None:
+			self.baseline_g2p_model.basic_net.to(self.compute_device)
 
 	def per_datum_ELBO(self,annot_data,freq_data,gene_data,num_particles=10,prior_only=False):
 		""" Computes the evidence lower bound (ELBO) for each observation in the dataset.
 
 		Parameters
 		----------
 		obs_data : torch.tensor
```

### Comparing `VAE_G2P-0.0.9/VAE_G2P/data.py` & `VAE_G2P-0.1.0/VAE_G2P/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 			freq_estimate=((num+prior_count)/(denom+prior_count*2.0))
 			for i,cp in enumerate(self.ordinal_cut_points):
 				if freq_estimate<=cp:
 					return i
 		else:
 			return self.ordinal_freq_map[symptom_freq_info]
 
-	def __init__(self,disease_labels,symptom_freq_pairs,disease_associated_genes,gene_info_table,ordinal_freq_upperlimits,training_data_fraction,validation_data_fraction,missing_label='NA',preprocess_symptom_counts=True,symptom_count_prior=1.0):
+	def __init__(self,disease_labels,symptom_freq_pairs,disease_associated_genes,ordinal_freq_upperlimits,training_data_fraction,validation_data_fraction,gene_info_table=None,missing_label='NA',preprocess_symptom_counts=True,symptom_count_prior=1.0):
 		"""Dataset that stores disease-symptom annotations as a sparse array that can be used for disease embedding.
 		
 		Args:
 		    disease_labels (Array of Strings): Strings that make up the index of the disease dataset
 		    symptom_freq_pairs (Array of iterables): Each list contains the symptoms-frequency pairs annotated to each disease. Symptoms-frequencies are stored as a tuple.
 		    ordinal_freq_map (Dictionary): Dictionary providing ordinal rank of each frequency used to describe the symptoms. 
 		    missing_label (str, optional): String used to denote missing frequency information.
@@ -81,16 +81,19 @@
 		
 		self.ordinal_cut_points=np.array(list(ordinal_freq_upperlimits.values()))
 		self.ordinal_freq_map=dict(zip(np.array(list(ordinal_freq_upperlimits.keys()))[np.argsort(self.ordinal_cut_points)],np.arange(self.ordinal_cut_points.shape[0])))
 		self.ordinal_cut_points=np.sort(self.ordinal_cut_points)
 		self.ordinal_freq_map[missing_label]=-1
 		self.num_ordinal_freqs = len(self.ordinal_freq_map)-1
 		self.missing_label=missing_label
+		if gene_info_table is None:
+			self.gene_info_table=pd.DataFrame([],index=disease_associated_genes)
+		else:
+			self.gene_info_table=gene_info_table
 
-		self.gene_info_table=gene_info_table
 		self.symptom_count_prior=symptom_count_prior
 
 		if preprocess_symptom_counts:
 			new_symptoms = orig_symp_values.apply(lambda x: [(self.symptom_map[y[0]],self._ProcessSymptomCounts(y[1],symptom_count_prior)) for y in x])
 			self.disease_table['SympFreqs']=new_symptoms
 		else:
 			raise ValueError("Direct modeling of symptoms counts not yet supported.")
@@ -219,15 +222,18 @@
 		symp_arrays=tuple(self._torchWrapper(x) for x in symp_arrays)
 		gene_arrays=self.ReturnGeneDataArrays([self.inverse_gene_map[x] for x in self.disease_table.loc[index]['MappedGenes'].values])
 		return symp_arrays+(gene_arrays,)
 
 	def ReturnGeneDataArrays(self,gene_list):
 		gene_arrays=self._build_gene_table_matrices(gene_list)
 		gene_arrays=tuple(self._torchWrapper(x) for x in gene_arrays)
-		return torch.cat(gene_arrays,axis=1)
+		if gene_arrays:
+			return torch.cat(gene_arrays,axis=1)
+		else:
+			None
 
 
 	def DropSymptoms(self,symptom_list):
 
 		oldSymptomToIntMap=self.symptom_map
 
 		allSymptoms=set(oldSymptomToIntMap.keys())
```

### Comparing `VAE_G2P-0.0.9/VAE_G2P/data_wrapper.py` & `VAE_G2P-0.1.0/VAE_G2P/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.9/VAE_G2P/networks.py` & `VAE_G2P-0.1.0/VAE_G2P/networks.py`

 * *Files identical despite different names*

### Comparing `VAE_G2P-0.0.9/VAE_G2P/optim.py` & `VAE_G2P-0.1.0/VAE_G2P/optim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import torch
 import pyro
 from pyro.infer import SVI
 from pyro.infer import Trace_ELBO
 from torch.utils import data
-from pyro.optim import AdamW
+from pyro.optim import AdamW,ClippedAdam
 from scipy.stats import linregress
 from pyro import poutine
 from collections import deque
 
 from .data_wrapper import TorchDataWrapper
 
 def rel_diff(curr,prev):
@@ -79,15 +79,15 @@
             ELBO error 
         """
         return abs(linregress(range(len(elbo_deque)),elbo_deque)[0]/np.mean(elbo_deque))
 
 
 
 
-    def __init__(self,vae_model,dataset_training_state,optimizationParameters={'learningRate': 0.05,'maxEpochs': 500,'numParticles':10},computeConfiguration={'device':None,'numDataLoaders':0}, **kwargs):
+    def __init__(self,vae_model,dataset_training_state,optimizationParameters={'initLearningRate': 0.01,'maxEpochs': 500,'numParticles':10,'finalLearningRate':0.001},computeConfiguration={'device':None,'numDataLoaders':0}, **kwargs):
         """
 
         This class implements a SGD optimizer, which uses mini-batches randomly sampled from a training dataset. To improve convergence rate and escape local minima, learning rate can be autommatically altered during inference. Note, given stochastic inference strategy coupled with possible re-starts, class tracks model perfomance and stores the best possible instance of the model obtained throughout the inference process.
 
                 vae_model-->The vae model to optimize
                 dataset_training_state-->DatasetTrainingState that holds clinical data and indices of the training and validation datasets.
 
@@ -116,16 +116,17 @@
         allKeywordArgs = list(kwargs.keys())
 
         self.vae_model=vae_model
         self.dataset_training_state=dataset_training_state
 
         #general optimization parameters
         self.maxEpochs=optimizationParameters['maxEpochs']
-        self.learningRate = optimizationParameters['learningRate']
+        self.initLearningRate = optimizationParameters['initLearningRate']
         self.numParticles = optimizationParameters['numParticles']
+        self.finalLearningRate = optimizationParameters['finalLearningRate']
 
         #compute resources parameters
         self.device=computeConfiguration['device']
         if self.device is None:
             self.device='cpu'
 
         else:
@@ -153,15 +154,14 @@
             self.KLAnnealingParams = {'initialTemp':1.0,'maxTemp':1.0,'fractionalDuration':1.0,'schedule': 'cosine'}
         else:
             self.KLAnnealingParams=kwargs['KLAnnealingParams']
             assert set(self.KLAnnealingParams.keys())==set(['initialTemp','maxTemp','fractionalDuration','schedule']),"KL Annealing Parameters must be dictionary with the following keys: 'initialTemp','maxTemp','fractionalDuration','schedule'"
 
 
 
-
     def BatchTrain(self,batch_size:int,errorTol:float = 1e-3,verbose=True,logFile=None,errorComputationWindow=None,early_stop_patience=5,monitor_validation=True):
         """
 
         Trains the VAE model using the mini-batches. This is the recommended method.
 
         Parameters
         ----------
@@ -206,87 +206,93 @@
 
             
 
         torchTrainingData=TorchDataWrapper(self.dataset_training_state,batch_size,index='Training')
         torchValidationData=TorchDataWrapper(self.dataset_training_state,batch_size,index='Validation')
 
 
-        sviFunction = SVI(self.vae_model.model,self.vae_model.guide,AdamW({'weight_decay':self.AdamW_Weight_Decay,'lr':self.learningRate}),loss=Trace_ELBO(num_particles=self.numParticles))
-
+        lrd=(self.finalLearningRate/self.initLearningRate)**(1/(self.maxEpochs*len(torchTrainingData)))
+        sviFunction = SVI(self.vae_model.model,self.vae_model.guide,ClippedAdam({'weight_decay':self.AdamW_Weight_Decay,'lr':self.initLearningRate,'lrd':lrd}),loss=Trace_ELBO(num_particles=self.numParticles))
         annealer=AnnealingScheduler(self.KLAnnealingParams['initialTemp'],self.KLAnnealingParams['maxTemp'],int(len(torchTrainingData)*(self.maxEpochs*self.KLAnnealingParams['fractionalDuration'])),self.KLAnnealingParams['schedule'])
 
         paramUpdateNum=0
 
         #initialize model states and scores
-        bestModelState=self.vae_model.package_state()
+        bestModelState=None
 
         #note, batch_size handled at the level of _TorchDatasetWrapper, not loader itself.
         trainingDataLoader = data.DataLoader(torchTrainingData,num_workers=self.num_dataloaders,collate_fn=collate_it)
         validationDataLoader = data.DataLoader(torchValidationData,num_workers=self.num_dataloaders,collate_fn=collate_it)
 
         avg_epoch_train_loss = 0.0
         self.vae_model.eval()
         for i,data_batch in enumerate(trainingDataLoader):
             if self.device.split(':')[0]!='cpu':
-                data_batch=tuple([x.to(self.device) for x in data_batch])
+                data_batch=tuple([x.to(self.device) if x is not None else None for x in data_batch])
 
             avg_epoch_train_loss+=sviFunction.evaluate_loss(*data_batch,minibatch_scale = (numTotalTrainingSamples/data_batch[0].shape[0]),annealing_factor=annealer.currentTemp(paramUpdateNum+1))
         avg_epoch_train_loss=avg_epoch_train_loss/(i+1)
         prev_train_loss=avg_epoch_train_loss
 
 
         avg_epoch_val_loss = 0.0
         for i,data_batch in enumerate(validationDataLoader):
             if self.device.split(':')[0]!='cpu':
-                data_batch=tuple([x.to(self.device) for x in data_batch])
+                data_batch=tuple([x.to(self.device) if x is not None else None for x in data_batch])
 
             avg_epoch_val_loss+=sviFunction.evaluate_loss(*data_batch,minibatch_scale = (numTotalValidationSamples/data_batch[0].shape[0]),annealing_factor=self.KLAnnealingParams['maxTemp'])
         avg_epoch_val_loss = avg_epoch_val_loss/(i+1)
         bestModelScore = np.inf
 
         elbo_window.append(prev_train_loss)
 
         early_stop_count=0
         for epoch in range(self.maxEpochs):
             torchTrainingData.shuffle_index()
             avg_epoch_train_loss = 0.0
             self.vae_model.train()
+            test=0.0
             for i,data_batch in enumerate(trainingDataLoader):
                 paramUpdateNum+=1
                 if self.device.split(':')[0]!='cpu':
-                    data_batch=tuple([x.to(self.device) for x in data_batch])
+                    data_batch=tuple([x.to(self.device) if x is not None else None for x in data_batch])
+
                 avg_epoch_train_loss+=sviFunction.step(*data_batch,minibatch_scale = (numTotalTrainingSamples/data_batch[0].shape[0]),annealing_factor=annealer.currentTemp(paramUpdateNum))
+
             avg_epoch_train_loss=avg_epoch_train_loss/(i+1.0)
 
             avg_epoch_val_loss = 0.0
             self.vae_model.eval()
             for i,data_batch in enumerate(validationDataLoader):
                 if self.device.split(':')[0]!='cpu':
-                    data_batch=tuple([x.to(self.device) for x in data_batch])
+                    data_batch=tuple([x.to(self.device) if x is not None else None for x in data_batch])
                 avg_epoch_val_loss+=sviFunction.evaluate_loss(*data_batch,minibatch_scale = (numTotalValidationSamples/data_batch[0].shape[0]),annealing_factor=self.KLAnnealingParams['maxTemp'])
             avg_epoch_val_loss=avg_epoch_val_loss/(i+1.0)
 
             if np.isnan(avg_epoch_val_loss) or np.isnan(avg_epoch_train_loss):
                 print("Warning: NaN detected during inference. Model unlikely to be fully optimized!")
                 break
 
-            if monitor_validation:
-                if avg_epoch_val_loss<bestModelScore:
-                    bestModelState = self.vae_model.package_state()
-                    bestModelScore = avg_epoch_val_loss
-                    early_stop_count=0
-                else:
-                    early_stop_count+=1 
-            else:
-                if avg_epoch_train_loss<bestModelScore:
-                    bestModelState = self.vae_model.package_state()
-                    bestModelScore = avg_epoch_train_loss
-                    early_stop_count=0
+                    
+            if annealer.currentTemp(paramUpdateNum)==self.KLAnnealingParams['maxTemp']:
+                if monitor_validation:
+                    if avg_epoch_val_loss<bestModelScore:
+                        bestModelState = self.vae_model.package_state()
+                        bestModelScore = avg_epoch_val_loss
+                        early_stop_count=0
+                    else:
+                        early_stop_count+=1 
                 else:
-                    early_stop_count+=1 
+                    if avg_epoch_train_loss<bestModelScore:
+                        bestModelState = self.vae_model.package_state()
+                        bestModelScore = avg_epoch_train_loss
+                        early_stop_count=0
+                    else:
+                        early_stop_count+=1 
+
 
 
             #track overall convergence
             trainLoss+=[avg_epoch_train_loss]
             validationLoss+=[avg_epoch_val_loss]
 
 
@@ -306,15 +312,15 @@
                     print("Model diverging after %03d epochs; stopping optimization. Current Loss (Train, Validation): %.4f, %.4f; Error: %.4e"%(epoch+1,trainLoss[-1],validationLoss[-1],errorVec[-1]))
                 if logFile!=None:
                     with open(logFile, "a") as f:
                         f.write("Model diverging after %03d epochs; stopping optimization. Current Loss (Train, Validation): %.4f, %.4f; Error: %.4e\n"%(epoch+1,trainLoss[-1],validationLoss[-1],errorVec[-1]))
                 break
 
 
-            if (avg_error < errorTol) or (med_error < errorTol) or (slope_error<errorTol):
+            if ((avg_error < errorTol) or (med_error < errorTol) or (slope_error<errorTol)) and (annealer.currentTemp(paramUpdateNum)==self.KLAnnealingParams['maxTemp']):
 
 
                 if verbose:
                     print("Optimization converged in %03d epochs; Current Loss (Train, Test): %.4f, %.4f; Error: %.4e"%(epoch+1,trainLoss[-1],validationLoss[-1],errorVec[-1]))
                 if logFile!=None:
                     with open(logFile, "a") as f:
                         f.write("Optimization converged in %03d epochs; Current Loss (Train, Test): %.4f, %.4f; Error: %.4e\n"%(epoch+1,trainLoss[-1],validationLoss[-1],errorVec[-1]))
```

### Comparing `VAE_G2P-0.0.9/VAE_G2P/vae_g2p.py` & `VAE_G2P-0.1.0/VAE_G2P/vae_g2p.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pandas as pd
 import numpy as np
 import torch
 import pickle
 import pyro
 import copy
+from scipy.stats import sem
 
 from .cvae_model import DiseaseCondVAE
-from .basic_g2p import BasicG2PModel
+from .basic_g2p import BasicG2PModel,BasicG2PMapLoss_Categorical
 from .data import GeneToPhenotypeDataset
 from .optim import AutoEncoderOptimizer
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
 
 
 class VAE_G2P:
 
 	def _readModelFromFile(self,fName):
 		with open(fName,'rb') as f:
 			model_dict = torch.load(f,map_location='cpu')
@@ -34,18 +35,22 @@
 			self.all_model_kwargs['encoder_hyperparameters']={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True}
 		if 'decoder_hyperparameters' not in self.all_model_kwargs.keys():
 			self.all_model_kwargs['decoder_hyperparameters']={'n_layers' : 2, 'n_hidden' : 64, 'dropout_rate': 0.1, 'use_batch_norm':True}
 
 		if 'missing_freq_priors' not in self.all_model_kwargs.keys():
 			self.all_model_kwargs['missing_freq_priors']=[0.0,3.0]
 
-	
-		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
+		if self.diseaseGeneDataset.aux_gene_info_table['return_dim'].sum()==0:
+			self.basic_g2p=None
+			self.isConditional=False
+		else:
+			self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
+			self.isConditional=True
 
-		self.vae_g2p_model=DiseaseCondVAE(self.numSymptoms,self.numFreqCats,self.nLatentDim,self.basic_g2p,isLinear=self.isLinear,encoder_hyperparameters=self.all_model_kwargs['encoder_hyperparameters'],decoder_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],missing_freq_prior_mean=self.all_model_kwargs['missing_freq_priors'][0],missing_freq_prior_scale=self.all_model_kwargs['missing_freq_priors'][1],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
+		self.vae_g2p_model=DiseaseCondVAE(self.numSymptoms,self.numFreqCats,self.nLatentDim,baseline_g2p_model=self.basic_g2p,isLinear=self.isLinear,encoder_hyperparameters=self.all_model_kwargs['encoder_hyperparameters'],decoder_hyperparameters=self.all_model_kwargs['decoder_hyperparameters'],missing_freq_prior_mean=self.all_model_kwargs['missing_freq_priors'][0],missing_freq_prior_scale=self.all_model_kwargs['missing_freq_priors'][1],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
 
 
 	def Fit(self,batch_size,logFile=None,verbose=True,monitor_validation=True,prior_model_state=None,**kwargs):
 		"""
 
 
 		Parameters
@@ -60,16 +65,19 @@
 
 		logFile: str, optional
 
 		    File to log model fitting process.
 
 		Keyword Parameters
 		----------
-		learningRate: float, optional
-		    Specifies the maximum learning rate used during inference. Default is 0.05
+		initLearningRate: float, optional
+		    Specifies the maximum learning rate used during inference. Default is 0.01
+
+		finalLearningRate: float, optional
+		    Specifies the final learning rate used during inference. Default is 0.001		 
 
 		errorTol: float, optional
 		    Error tolerance in ELBO (computed on held out validation data) to determine convergence. Default is 1e-4.
 
 		numParticles: int, optional
 		    Number of particles (ie random samples) used to approximate gradient. Default is 1. Computational cost increases linearly with value.
 
@@ -101,18 +109,23 @@
 		"""
 
 
 		######### Parse Keyword Arguments #########
 		allKeywordArgs = list(kwargs.keys())
 
 
-		if 'learningRate' in allKeywordArgs:
-		    learningRate=kwargs['learningRate']
+		if 'initLearningRate' in allKeywordArgs:
+		    initLearningRate=kwargs['initLearningRate']
 		else:
-		    learningRate=0.01
+		    initLearningRate=0.01
+
+		if 'finalLearningRate' in allKeywordArgs:
+		    finalLearningRate=kwargs['finalLearningRate']
+		else:
+		    finalLearningRate=0.001
 
 
 		if 'errorTol' in allKeywordArgs:
 		    errorTol=kwargs['errorTol']
 		else:
 		    errorTol=1e-4
 
@@ -142,33 +155,34 @@
 
 		if 'KLAnnealingParams' in allKeywordArgs:
 		    KLAnnealingParams=kwargs['KLAnnealingParams']
 		    assert set(KLAnnealingParams.keys())==set(['initialTemp','maxTemp','fractionalDuration','schedule']),"KL Annealing Parameters must be dictionary with the following keys: 'initialTemp','maxTemp','fractionalDuration','schedule'"
 		else:
 		    KLAnnealingParams={'initialTemp':1.0,'maxTemp':1.0,'fractionalDuration':1.0,'schedule': 'cosine'}
 
-
 		if 'EarlyStopPatience' in allKeywordArgs:
 			EarlyStopPatience=kwargs['EarlyStopPatience']
 		else:
 			EarlyStopPatience=10
 
 
 		pyro.clear_param_store()
-		if prior_model_state is None:
-			self.basic_g2p.Fit(batch_size,learningRate,maxEpochs,errorTol,compute_device=computeDevice,numDataLoaders=numDataLoaders,early_stop_patience=EarlyStopPatience,monitor_validation=False)
-		else:
-			self.basic_g2p.LoadModel(prior_model_state)
+		if self.isConditional==True:
+			if prior_model_state is None:
+				self.basic_g2p.Fit(batch_size,initLearningRate,maxEpochs,errorTol,compute_device=computeDevice,numDataLoaders=numDataLoaders,early_stop_patience=EarlyStopPatience,monitor_validation=False)
+			else:
+				self.basic_g2p.LoadModel(prior_model_state)
 
-
-		optimizer=AutoEncoderOptimizer(self.vae_g2p_model,self.diseaseGeneDataset,optimizationParameters={'learningRate': learningRate,'maxEpochs': maxEpochs,'numParticles':numParticles},computeConfiguration={'device':computeDevice,'numDataLoaders':numDataLoaders},KLAnnealingParams=KLAnnealingParams)
+		optimizer=AutoEncoderOptimizer(self.vae_g2p_model,self.diseaseGeneDataset,optimizationParameters={'initLearningRate': initLearningRate,'maxEpochs': maxEpochs,'numParticles':numParticles,'finalLearningRate':finalLearningRate},computeConfiguration={'device':computeDevice,'numDataLoaders':numDataLoaders},KLAnnealingParams=KLAnnealingParams)
 		output=optimizer.BatchTrain(batch_size,errorTol=errorTol,verbose=verbose,logFile=logFile,monitor_validation=monitor_validation,early_stop_patience=EarlyStopPatience)
 		return output
 
 	def PredictEmbedFromGeneOnly(self,gene_list,returnStdErrors=False):
+		if self.isConditional==False:
+			raise ValueError("Predictions from genes are only possible for a conditional model that is fed gene-specific information.")
 		assert len(set(gene_list).difference(self.diseaseGeneDataset.gene_map.keys()))==0,"The following genes are not in the embedding table: {0:s}".format(','.join(list(set(gene_vec).difference(self.diseaseGeneDataset.gene_map.keys()))))
 
 		gene_data=self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list)
 		modes_for_prior = torch.cat(self.vae_g2p_model.baseline_g2p_model.basic_net(gene_data),axis=1)
 		p_m,p_std = self.vae_g2p_model.prior_model(torch.cat((modes_for_prior,gene_data),axis=1))
 
 		output_table={'Genes':gene_list,'Embeddings':[x for x in p_m.detach().numpy()]}
@@ -176,223 +190,212 @@
 		if returnStdErrors:
 			output_table['Std Errors']=[x for x in p_std.detach().numpy()]
 		output_table=pd.DataFrame(output_table)
 		output_table.set_index('Genes',inplace=True)
 		return output_table
 
 
-	def PredictSymptomsFromGeneOnly(self,gene_list,numSamples=0):
+	def PredictSymptomsFromGeneOnly(self,gene_list,num_particles=0):
 		embeds=self.PredictEmbedFromGeneOnly(gene_list,returnStdErrors=True)
 		z_loc=np.vstack(embeds.loc[gene_list]['Embeddings'].values)
 		z_scale=np.vstack(embeds.loc[gene_list]['Std Errors'].values)
-		if numSamples==0:
+		if num_particles==0:
 			symptom_probs=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder.forward(torch.tensor(z_loc))).detach().numpy()
 
 			symptom_freqs=torch.exp(pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(torch.tensor(z_loc)),self.vae_g2p_model.cut_points).logits).detach().numpy()
 		else:
-			samples_from_priors = torch.normal(torch.tensor(z_loc)*torch.ones((numSamples,z_loc.shape[0],z_loc.shape[1])),torch.tensor(z_scale)*torch.ones((numSamples,z_loc.shape[0],z_loc.shape[1])))
+			samples_from_priors = torch.normal(torch.tensor(z_loc)*torch.ones((num_particles,z_loc.shape[0],z_loc.shape[1])),torch.tensor(z_scale)*torch.ones((num_particles,z_loc.shape[0],z_loc.shape[1])))
 
 			symptom_probs=np.zeros((len(gene_list),self.numSymptoms))
 			symptom_freqs=np.zeros((len(gene_list),self.numSymptoms,self.numFreqCats))
 
-			for i in range(numSamples):
-				symptom_probs+=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder.forward(samples_from_priors[i])).detach().numpy()/numSamples
-				symptom_freqs+=torch.exp(pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(samples_from_priors[i]),self.vae_g2p_model.cut_points).logits).detach().numpy()/numSamples
+			for i in range(num_particles):
+				symptom_probs+=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder.forward(samples_from_priors[i])).detach().numpy()/num_particles
+				symptom_freqs+=torch.exp(pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(samples_from_priors[i]),self.vae_g2p_model.cut_points).logits).detach().numpy()/num_particles
 
 		output_table=pd.DataFrame([],index=self.diseaseGeneDataset.symptom_map.keys(),columns=gene_list)
 		for i,gene in enumerate(gene_list):
 			output_table[gene]=list(zip(symptom_probs[i],symptom_freqs[i]))
 		return output_table
 
 	
 
-	def _per_datam_elbo(self,hpo_freq_pairs,gene_list,num_particles=10):
+	def _per_datum_elbo(self,hpo_freq_pairs,gene_list,num_particles=10):
 		assert isinstance(hpo_freq_pairs,list),"The provided HPO-frequncy pairs must be an interable of ('HPO Symptom','Frequency') nested within a list."
-
-		assert isinstance(gene_list,list),"Conditional VAE model expects a list of genes in order to compute ELBO"
-		assert len(hpo_freq_pairs)==len(gene_list) or (len(hpo_freq_pairs)==1 or len(gene_list)==1),"Number of provided symptom-frequency pair datasets must equal number of genes, unless number of genes or the number of symptom-frequency pair datasets is equal to 1, at which point the data type with length 1 is broadcasted to the same size as the other dataset."
-
-		#generate data tensors, allows broadcasting 
-		annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-		freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-
-		if len(gene_list)<len(hpo_freq_pairs):
-			gene_list=gene_list*len(hpo_freq_pairs)
-		elif len(gene_list)>len(hpo_freq_pairs):
-			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
+		if self.isConditional==True:
+			assert isinstance(gene_list,list),"Conditional VAE model expects a list of genes in order to compute ELBO"
+			assert len(hpo_freq_pairs)==len(gene_list) or (len(hpo_freq_pairs)==1 or len(gene_list)==1),"Number of provided symptom-frequency pair datasets must equal number of genes, unless number of genes or the number of symptom-frequency pair datasets is equal to 1, at which point the data type with length 1 is broadcasted to the same size as the other dataset."
+			annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
+			freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
+			if len(gene_list)<len(hpo_freq_pairs):
+				gene_list=gene_list*len(hpo_freq_pairs)
+			elif len(gene_list)>len(hpo_freq_pairs):
+				hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
+		else:
+			gene_list=[]
+			annot_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
+			freq_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
 
 		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
 			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
 			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
 			annot_array[t,idx_vec]=1.0
 			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
-
-		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
+		if self.isConditional==True:
+			data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
+		else:
+			data=(annot_array,freq_array,None)
 
 		elbo=self.vae_g2p_model.per_datum_ELBO(*data,num_particles=num_particles)
 		return elbo.detach().numpy().ravel()
 
-	def PerplexCompare(self,hpo_freq_pairs,gene_list,index=None,num_particles=10):
-		perplex_vec = -1.0*self._per_datam_elbo(hpo_freq_pairs,gene_list,num_particles=num_particles)
-		model_compare_results=self.basic_g2p.PerplexCompareNull(hpo_freq_pairs,gene_list)
-		model_compare_results['VAE_G2P Perplex.']=perplex_vec
-		model_compare_results['VAE_G2P-BasicG2PModel']=model_compare_results['VAE_G2P Perplex.']-model_compare_results['BasicG2PModel Perplex.']
-		model_compare_results['VAE_G2P-Null']=model_compare_results['VAE_G2P Perplex.']-model_compare_results['Null Perplex.']
-		model_compare_results['Genes']=gene_list
-		model_compare_results=pd.DataFrame(model_compare_results)
+	def PerplexCompare(self,hpo_freq_pairs,gene_list=None,index=None,num_particles=10):
+
+		perplex_vec = -1.0*self._per_datum_elbo(hpo_freq_pairs,gene_list=gene_list,num_particles=num_particles)
+		if self.isConditional==True:
+			model_compare_results=self.basic_g2p.PerplexCompareNull(hpo_freq_pairs,gene_list)
+			model_compare_results['VAE_G2P Perplex.']=perplex_vec
+			model_compare_results['VAE_G2P-BasicG2PModel']=model_compare_results['VAE_G2P Perplex.']-model_compare_results['BasicG2PModel Perplex.']
+			model_compare_results['VAE_G2P-Null']=model_compare_results['VAE_G2P Perplex.']-model_compare_results['Null Perplex.']
+			model_compare_results['Genes']=gene_list
+			model_compare_results=pd.DataFrame(model_compare_results)
+		else:
+
+			annot_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
+			freq_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
+			for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
+			    idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
+			    freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
+			    annot_array[t,idx_vec]=1
+			    freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
+
+			null_model_log_odds=tuple(torch.logit(self.diseaseGeneDataset._torchWrapper(x)).unsqueeze(dim=0) for x in self.diseaseGeneDataset.InferNullModel().values())
+			output=np.zeros((perplex_vec.shape[0],3))
+			perplex_function_null=BasicG2PMapLoss_Categorical()
+			for i in range(output.shape[0]):
+				output[i,0]=perplex_vec[i]
+				output[i,1]=perplex_function_null(null_model_log_odds[0],null_model_log_odds[1],null_model_log_odds[2], annot_array[i:i+1],freq_array[i:i+1]).detach().item()
+				output[i,2]=output[i,0]-output[i,1]
+
+			model_compare_results={}
+			model_compare_results['VAE_G2P Perplex.']=output[:,0]
+			model_compare_results['Null Perplex.']=output[:,1]
+			model_compare_results['VAE_G2P-Null']=output[:,2]
+			model_compare_results=pd.DataFrame(model_compare_results)
+
 		if index is not None:
 			model_compare_results['Index']=index
 		else:
-			model_compare_results['Index']=['Dis_{0:d}'.format(x) for x in range(len(gene_list))]
+			model_compare_results['Index']=['IDX_{0:d}'.format(x) for x in range(len(hpo_freq_pairs))]
 		model_compare_results.set_index('Index',inplace=True)
 		return model_compare_results
 
 
-	def EmbedDisease(self,hpo_freq_pairs,gene_list,index=None,returnStdErrors=False):
-		assert isinstance(hpo_freq_pairs,list),"The provided HPO-frequncy pairs must be an interable of ('HPO Symptom','Frequenc') nested within a list."
-		assert isinstance(gene_list,list),"Conditional VAE model expects a list of genes in order to compute ELBO"
-		assert len(hpo_freq_pairs)==len(gene_list) or (len(hpo_freq_pairs)==1 or len(gene_list)==1),"Number of provided symptom-frequency pair datasets must equal number of genes, unless number of genes or the number of symptom-frequency pair datasets is equal to 1, at which point the data type with length 1 is broadcasted to the same size as the other dataset."
-
-		#generate data tensors, allows broadcasting 
-		annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-		freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-
-		if len(gene_list)<len(hpo_freq_pairs):
-			gene_list=gene_list*len(hpo_freq_pairs)
-		elif len(gene_list)>len(hpo_freq_pairs):
-			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
-
-		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
-			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
-			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
-			annot_array[t,idx_vec]=1.0
-			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
-
-		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
-		p_m,p_std=self.vae_g2p_model.posterior_latent_state(*data)
 
-		if index is None:
-			index=['Dis_{0:d}'.format(x) for x in range(len(gene_list))]
-		output_table={'Index':index,'Gene':gene_list,'Embeddings':[x for x in p_m.detach().numpy()]}
 
-		if returnStdErrors:
-			output_table['Std Errors']=[x for x in p_std.detach().numpy()]
-		output_table=pd.DataFrame(output_table)
-		output_table.set_index('Index',inplace=True)
-		return output_table
-
-	def _embedDisease(self,hpo_freq_pairs,gene_list,returnStdErrors=False):
-		assert isinstance(hpo_freq_pairs,list),"The provided HPO-frequncy pairs must be an interable of ('HPO Symptom','Frequenc') nested within a list."
-		assert isinstance(gene_list,list),"Conditional VAE model expects a list of genes in order to compute ELBO"
-		assert len(hpo_freq_pairs)==len(gene_list) or (len(hpo_freq_pairs)==1 or len(gene_list)==1),"Number of provided symptom-frequency pair datasets must equal number of genes, unless number of genes or the number of symptom-frequency pair datasets is equal to 1, at which point the data type with length 1 is broadcasted to the same size as the other dataset."
-
-		#generate data tensors, allows broadcasting 
-		annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-		freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
-
-		if len(gene_list)<len(hpo_freq_pairs):
-			gene_list=gene_list*len(hpo_freq_pairs)
-		elif len(gene_list)>len(hpo_freq_pairs):
-			hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
+	def _embedDisease(self,hpo_freq_pairs,gene_list=None):
+		assert isinstance(hpo_freq_pairs,list),"The provided HPO-frequncy pairs must be an interable of ('HPO Symptom','Frequency') nested within a list."
+		if self.isConditional==True:
+			assert isinstance(gene_list,list),"Conditional VAE model expects a list of genes in order to compute ELBO"
+			assert len(hpo_freq_pairs)==len(gene_list) or (len(hpo_freq_pairs)==1 or len(gene_list)==1),"Number of provided symptom-frequency pair datasets must equal number of genes, unless number of genes or the number of symptom-frequency pair datasets is equal to 1, at which point the data type with length 1 is broadcasted to the same size as the other dataset."
+			annot_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
+			freq_array=torch.zeros((max(len(hpo_freq_pairs),len(gene_list)),self.numSymptoms),dtype=torch.float32)
+			if len(gene_list)<len(hpo_freq_pairs):
+				gene_list=gene_list*len(hpo_freq_pairs)
+			elif len(gene_list)>len(hpo_freq_pairs):
+				hpo_freq_pairs=hpo_freq_pairs*len(gene_list)
+		else:
+			assert gene_list is None,"Passing gene list to a vanilla VAE model is not allowed."
+			gene_list=[]
+			annot_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
+			freq_array=torch.zeros((len(hpo_freq_pairs),self.numSymptoms),dtype=torch.float32)
 
 		for t,hpo_freq_vec in enumerate(hpo_freq_pairs):
 			idx_vec=[self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec]
 			freq_vec=[self.diseaseGeneDataset._ProcessSymptomCounts(x[1],self.diseaseGeneDataset.symptom_count_prior) for x in hpo_freq_vec]
 			annot_array[t,idx_vec]=1.0
 			freq_array[t,idx_vec]=torch.tensor(freq_vec,dtype=torch.float32)
 
-		data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
-		p_m,p_std=self.vae_g2p_model.posterior_latent_state(*data)
-
-		if returnStdErrors:
-			return p_m.detach().numpy(),p_std.detach().numpy()
+		if self.isConditional==True:
+			data=(annot_array,freq_array,self.diseaseGeneDataset.ReturnGeneDataArrays(gene_list))
 		else:
-			return p_m.detach().numpy()
-
+			data=(annot_array,freq_array,None)
 
-	def EstimateMissingAnnotationRates(self,hpo_freq_pairs,gene_list,index=None):
-		assert len(hpo_freq_pairs)==len(gene_list),"Expect length of HPO-Freqency Pair sets and gene lists to be the same."
-		mapping_dict={}
-		for i,hpo_freq_vec in enumerate(hpo_freq_pairs):
-			mapping_dict[gene_list[i]]=torch.tensor([self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec],dtype=torch.long)
-
-		post_mean=self._embedDisease(hpo_freq_pairs,gene_list=gene_list,returnStdErrors=False)
-
-		if index is None:
-			index=['Dis_{0:d}'.format(x) for x in range(len(gene_list))]
-		output_table={'Index':index,'Gene':gene_list,'Missing Annot. Rates':[]}
-		for i,post_vec in enumerate(post_mean):
-			embed_tensor=torch.tensor(post_vec,dtype=torch.float32)
-			pred_missing_full=self.vae_g2p_model.missing_freq_disease_decoder(embed_tensor)+self.vae_g2p_model.missing_freq_intercepts_post_mean
-			pred_missing=torch.sigmoid(pred_missing_full[mapping_dict[gene_list[i]]]).detach().numpy()
-			output_table['Missing Annot. Rates']+=[list(zip([self.diseaseGeneDataset.inverse_symptom_map[x] for x in mapping_dict[gene_list[i]].detach().numpy()],pred_missing))]
-		output_table=pd.DataFrame(output_table)
-		output_table.set_index('Index',inplace=True)
-		return output_table
+		p_m,p_std=self.vae_g2p_model.posterior_latent_state(*data)
 
+		return p_m.detach().numpy(),p_std.detach().numpy()
 
-	def ImputeMissingSymptomFrequencies(self,hpo_freq_pairs,gene_list,index=None):
-		assert len(hpo_freq_pairs)==len(gene_list),"Expect length of HPO-Freqency Pair sets and gene lists to be the same."
-		mapping_dict={}
-		for i,hpo_freq_vec in enumerate(hpo_freq_pairs):
-			mapping_dict[gene_list[i]]=torch.tensor([self.diseaseGeneDataset.symptom_map[x[0]] for x in hpo_freq_vec if x[1]==self.diseaseGeneDataset.missing_label],dtype=torch.long)
 
-		post_mean=self._embedDisease(hpo_freq_pairs,gene_list,returnStdErrors=False)
+	def EmbedDisease(self,hpo_freq_pairs,gene_list=None,index=None,returnStdErrors=False):
 
+		pm,pstd=self._embedDisease(hpo_freq_pairs,gene_list)
 
 		if index is None:
-			index=['Dis_{0:d}'.format(x) for x in range(len(gene_list))]
-		output_table={'Index':index,'Gene':gene_list,'Missing Freqencies':[]}
-		for i,post_vec in enumerate(post_mean):
-			embed_tensor=torch.tensor(post_vec,dtype=torch.float32)
-			pred_class_full=pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(embed_tensor.unsqueeze(dim=0)),self.vae_g2p_model.cut_points).logits.squeeze(dim=0)
-			pred_annots=torch.exp(pred_class_full[mapping_dict[gene_list[i]],:]).detach().numpy()
-			output_table['Missing Freqencies']+=[list(zip([self.diseaseGeneDataset.inverse_symptom_map[x] for x in mapping_dict[gene_list[i]].detach().numpy()],pred_annots))]
+			index=['IDX_{0:d}'.format(x) for x in range(len(hpo_freq_pairs))]
+		if gene_list is None:
+			gene_list=['NA']*len(hpo_freq_pairs)
+		output_table={'Index':index,'Gene':gene_list,'Embeddings':[x for x in pm]}
+		if returnStdErrors:
+			output_table['Std Errors']=[x for x in pstd]
+
 		output_table=pd.DataFrame(output_table)
 		output_table.set_index('Index',inplace=True)
 		return output_table
 
-	def SuggestNewSymptoms(self,hpo_freq_pairs,gene_list,annot_rate_threshold=0.0,index=None):
-		assert len(hpo_freq_pairs)==len(gene_list),"Expect length of HPO-Freqency Pair sets and gene lists to be the same."
+	def EstimateAnnotationRates(self,hpo_freq_pairs,gene_list=None,index=None,estimateStdError=False,num_particles=100):
+		if estimateStdError==False:
+			output_table=self.EmbedDisease(hpo_freq_pairs,gene_list=gene_list,index=index,returnStdErrors=False)
+		else:
+			output_table=self.EmbedDisease(hpo_freq_pairs,gene_list=gene_list,index=index,returnStdErrors=True)
+
+		annot_table=output_table[['Gene']].copy()
+		annot_table['Annot. Rates']=[pd.NA for i in range(output_table.shape[0])]
+
+		for idx in output_table.index:
+			embed_tensor=torch.tensor(output_table.loc[idx]['Embeddings'],dtype=torch.float32).unsqueeze(0)
+			if estimateStdError==False:
+				pred_annots=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder(embed_tensor)).detach().numpy().squeeze(0)
+				annot_table.loc[idx]['Annot. Rates']=dict(zip([self.diseaseGeneDataset.inverse_symptom_map[x] for x in range(pred_annots.shape[0])],pred_annots))
+
+			else:
+				embed_scale=torch.tensor(output_table.loc[idx]['Std Errors'],dtype=torch.float32).unsqueeze(0)
+				samples=torch.normal(torch.ones(num_particles,embed_tensor.shape[0])*embed_tensor,torch.ones(num_particles,embed_tensor.shape[0])*embed_scale)
+				pred_annots_all=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder(samples)).detach().numpy()
+				pred_annots=list(zip(list(pred_annots_all.mean(axis=0)),list(sem(pred_annots_all,axis=0))))
 
-		mapping_dict={}
-		for i,hpo_freq_vec in enumerate(hpo_freq_pairs):
-			mapping_dict[gene_list[i]]=set([x[0] for x in hpo_freq_vec])
+				annot_table.loc[idx]['Annot. Rates']=dict(zip([self.diseaseGeneDataset.inverse_symptom_map[x] for x in range(len(pred_annots))],pred_annots))
+			
+		return annot_table
 
-		post_mean=self._embedDisease(hpo_freq_pairs,gene_list,returnStdErrors=False)
 
-		if index is None:
-			index=['Dis_{0:d}'.format(x) for x in range(len(gene_list))]
-		output_table={'Index':index,'Gene':gene_list,'New Symptoms':[]}
-		for i,post_vec in enumerate(post_mean):
-			embed_tensor=torch.tensor(post_vec,dtype=torch.float32)
-			pred_symptoms=torch.sigmoid(self.vae_g2p_model.symptom_annotation_decoder(embed_tensor.unsqueeze(dim=0)).squeeze(dim=0)).detach().numpy()
-			pred_class_full=pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(embed_tensor.unsqueeze(dim=0)),self.vae_g2p_model.cut_points).logits.squeeze(dim=0)
-			pred_class_full=torch.exp(pred_class_full).detach().numpy()
-
-			allowed_symptoms=np.arange(self.numSymptoms)
-			allowed_symptoms=allowed_symptoms[pred_symptoms>=annot_rate_threshold]
-			pred_class_full=pred_class_full[pred_symptoms>=annot_rate_threshold]
-			pred_symptoms=pred_symptoms[pred_symptoms>=annot_rate_threshold]
+	def EstimateSymptomFrequencies(self,hpo_freq_pairs,gene_list=None,index=None,estimateStdError=False,num_particles=100):
+		if estimateStdError==False:
+			output_table=self.EmbedDisease(hpo_freq_pairs,gene_list=gene_list,index=index,returnStdErrors=False)
+		else:
+			output_table=self.EmbedDisease(hpo_freq_pairs,gene_list=gene_list,index=index,returnStdErrors=True)
+
+
+		symptom_table=output_table[['Gene']].copy()
+		symptom_table['Symptom Freq.']=[pd.NA for i in range(output_table.shape[0])]
+		for idx in output_table.index:
+			embed_tensor=torch.tensor(output_table.loc[idx]['Embeddings'],dtype=torch.float32).unsqueeze(0)
+			if estimateStdError==False:
+				pred_class_full=pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(embed_tensor),self.vae_g2p_model.cut_points).logits.squeeze(dim=0)
+				pred_annots=torch.exp(pred_class_full).detach().numpy()
+			else:
+				embed_scale=torch.tensor(output_table.loc[idx]['Std Errors'],dtype=torch.float32).unsqueeze(0)
+				samples=torch.normal(torch.ones(num_particles,embed_tensor.shape[0])*embed_tensor,torch.ones(num_particles,embed_tensor.shape[0])*embed_scale)
+				pred_class_full=pyro.distributions.OrderedLogistic(self.vae_g2p_model.symptom_frequency_decoder(samples),self.vae_g2p_model.cut_points).logits.squeeze(dim=0)
 
+				pred_annots_all=torch.exp(pred_class_full).detach().numpy()
+				pred_annots=list(zip(pred_annots_all.mean(axis=0),sem(pred_annots_all,axis=0)))
 			
-			allowed_symptoms=allowed_symptoms[np.argsort(pred_symptoms)[::-1]]
-			pred_class_full=pred_class_full[np.argsort(pred_symptoms)[::-1]]
-			pred_symptoms=np.sort(pred_symptoms)[::-1]
-			output_vec=[]
-
-			for j in range(allowed_symptoms.shape[0]):
-				symptom=self.diseaseGeneDataset.inverse_symptom_map[allowed_symptoms[j]]
-				if symptom not in mapping_dict[gene_list[i]]:
-					output_vec+=[(symptom,pred_symptoms[j],pred_class_full[j])]
-			output_table['New Symptoms']+=[output_vec]
+			symptom_table.loc[idx]['Symptom Freq.']=dict(zip([self.diseaseGeneDataset.inverse_symptom_map[x] for x in range(len(pred_annots))],pred_annots))
+		return symptom_table
 
-		output_table=pd.DataFrame(output_table)
-		output_table.set_index('Index',inplace=True)
-		return output_table
 
 
 
 
 	def LoadModel(self,stored_model):
 		"""
 		Loads previously fit model either from a dictionary (generated using PackageModel) or from a file path (with file constructed using PackageModel)
@@ -407,15 +410,18 @@
 
 		"""
 		if not isinstance(stored_model,dict):
 			assert isinstance(stored_model,str),"Expects file name if not provided with dictionary."
 			stored_model = self._readModelFromFile(stored_model)
 
 		assert set(stored_model.keys())==set(['model_state','meta_data','variational_post_params','baseline_g2p_model']),"Model dictionary must contain the following elements: 'model_state','meta_data','baseline_g2p_model'"
-		self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=stored_model['meta_data']['all_model_kwargs']['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
+		if self.diseaseGeneDataset.aux_gene_info_table['return_dim'].sum()>0:
+			self.basic_g2p=BasicG2PModel(self.diseaseGeneDataset,network_hyperparameters=stored_model['meta_data']['all_model_kwargs']['decoder_hyperparameters'],cut_points=self.diseaseGeneDataset.ordinal_cut_points[:-1])
+		else:
+			self.basic_g2p=None
 		self.vae_g2p_model=DiseaseCondVAE(
 			stored_model['meta_data']['numSymptoms'],
 			stored_model['meta_data']['numFreqCats'],
 			stored_model['meta_data']['nLatentDim'],
 			self.basic_g2p,
 			isLinear=stored_model['meta_data']['isLinear'],
 			encoder_hyperparameters=stored_model['meta_data']['all_model_kwargs']['encoder_hyperparameters'],
```

### Comparing `VAE_G2P-0.0.9/setup.py` & `VAE_G2P-0.1.0/setup.py`

 * *Files identical despite different names*

