# Comparing `tmp/easy_mitk-0.0.1.tar.gz` & `tmp/easy_mitk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/app/sdk/easy-mitk/dist/.tmp-0fyogrt7/easy_mitk-0.0.1.tar", last modified: Fri May  5 11:21:07 2023, max compression
+gzip compressed data, was "/app/sdk/easy-mitk/dist/.tmp-l1rfdq5k/easy_mitk-0.0.2.tar", last modified: Sat May  6 16:01:00 2023, max compression
```

## Comparing `easy_mitk-0.0.1.tar` & `easy_mitk-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1066 2023-05-03 11:31:57.000000 easy_mitk-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-03 11:32:27.000000 easy_mitk-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk/
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 11:32:27.000000 easy_mitk-0.0.1/easy_mitk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21152 2023-05-04 10:18:46.000000 easy_mitk-0.0.1/easy_mitk/dicom.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-03 15:55:58.000000 easy_mitk-0.0.1/easy_mitk/measure.py
--rw-r--r--   0 root         (0) root         (0)      240 2023-05-03 11:46:05.000000 easy_mitk-0.0.1/easy_mitk/nifti.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:32:27.000000 easy_mitk-0.0.1/easy_mitk/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1290 2023-05-03 11:32:27.000000 easy_mitk-0.0.1/easy_mitk/utils/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/easy_mitk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-05-03 11:32:27.000000 easy_mitk-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      730 2023-05-05 11:20:54.000000 easy_mitk-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:21:07.000000 easy_mitk-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-03 11:33:31.000000 easy_mitk-0.0.1/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-05-03 15:28:18.000000 easy_mitk-0.0.1/tests/test_measure.py
--rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 11:32:28.000000 easy_mitk-0.0.1/tests/test_torch_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-03 11:31:57.000000 easy_mitk-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-06 15:55:55.000000 easy_mitk-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/easy_mitk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22752 2023-05-06 15:51:39.000000 easy_mitk-0.0.2/easy_mitk/dicom.py
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-05-06 15:18:42.000000 easy_mitk-0.0.2/easy_mitk/measure.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-06 15:52:33.000000 easy_mitk-0.0.2/easy_mitk/nifti.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/easy_mitk/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-05-06 15:54:22.000000 easy_mitk-0.0.2/easy_mitk/utils/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/easy_mitk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-05-03 11:32:27.000000 easy_mitk-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      739 2023-05-06 15:59:15.000000 easy_mitk-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 16:01:00.000000 easy_mitk-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-05-03 11:33:31.000000 easy_mitk-0.0.2/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-03 15:28:18.000000 easy_mitk-0.0.2/tests/test_measure.py
+-rw-r--r--   0 root         (0) root         (0)      193 2023-05-03 11:32:28.000000 easy_mitk-0.0.2/tests/test_torch_model.py
```

### Comparing `easy_mitk-0.0.1/LICENSE` & `easy_mitk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.1/easy_mitk/dicom.py` & `easy_mitk-0.0.2/easy_mitk/dicom.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,31 +12,46 @@
 from nibabel import nifti1
 from pydicom import Dataset, Sequence, dataset, uid
 from rle import encode_pixel_data
 
 
 def get_slice_location(dcm: Dataset) -> float:
     """
-    Get stack position from the number
+    Get stack position from the SliceLocation.
     :param dcm: DICOM Dataset
     :return:
     """
     return float(dcm.SliceLocation)
 
 
-def dcm2nii(dcm_dir: os.PathLike, save_path: os.PathLike = None) -> nifti1.Nifti1Image:
+def dcm2nii(dcm_dir: os.PathLike, save_path: os.PathLike) -> nifti1.Nifti1Image:
+    """
+    Convert DICOM image to NIfTI by dicom2nifti.
+    使用dicom2nifti将DICOM图像转为NIfTI。
+
+    Args:
+        dcm_dir (os.PathLike): _description_
+        save_path (os.PathLike): _description_
+
+    Returns:
+        nifti1.Nifti1Image: _description_
+    """
     # TODO 参考dicom2nifti，但要减少IO
-    if save_path:
-        os.makedirs(os.path.dirname(save_path), exist_ok=True)
-        nii = dicom2nifti.dicom_series_to_nifti(dcm_dir, save_path)['NII']
+    os.makedirs(os.path.dirname(save_path), exist_ok=True)
+    nii = dicom2nifti.dicom_series_to_nifti(dcm_dir, save_path)['NII']
     return nii
 
 
 def dcm2nii2(dcms: List[Dataset], save_path: os.PathLike = None) -> nifti1.Nifti1Image:
-    """当前只支持水平位扫描方向的图像转换
+    """
+    当前只支持水平位扫描方向的图像转换，且不关心图像的方向，只关心图像的内容和像素间距.
+    Currently only support scan along the axial direction，and does not care about the direction 
+    but the content and the pixel spacing of the image.
+
+    TODO 还是关心一下方向，保证affine计算正确
 
     Args:
         dcm_list (List[Dataset]): _description_
         save_path (os.PathLike, optional): _description_. Defaults to None.
 
     Returns:
         nifti1.Nifti1Image: _description_
@@ -52,15 +67,17 @@
     return nii
 
 # 允许与Z轴有10度偏差，cos(80度) = 0.17
 SLOPE_TOLERATE = 0.17
 
 
 def sort_slice_by_position(dcms: List[Dataset]) -> List[Dataset]:
-    """increase by z axis
+    """
+    沿着扫描方向递增。
+    Increment in the direction of the scan.
 
     Args:
         dcms (List[Dataset]): _description_
     """
     assert len(dcms) >= 2, '至少需要两个DICOM文件'
     filtered_dcm = []
     # Remove invalid images
@@ -78,29 +95,44 @@
     if len(filtered_dcm) < 1:
         raise Exception('No valid image found')
     filtered_dcm.sort(key=lambda x: x.ImagePositionPatient[2])
     return filtered_dcm
 
 
 def load_series(dcm_dir: os.PathLike) -> List[Dataset]:
-    """加载DICOM之后会根据空间坐标对每个图像进行排序
+    """
+    加载DICOM序列，并根据ImagePositionPatient对每个图像切片进行排序。
+    Load DICOM series and sort every image slice by ImagePositionPatient.
 
     Args:
         dicom_dir (os.PathLike): _description_
 
     Returns:
         List[Dataset]: _description_
     """
     dcms = []
     for f in glob(f'{dcm_dir}/*'):
         dcms.append(pydicom.dcmread(f))
     return sort_slice_by_position(dcms)
 
 
 def get_affine(dcms: List[Dataset], load_pixel_arr=True) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Compute affine matrix from DICOM.
+    从DICOM文件计算affine。
+
+    TODO 还是要关心一下方向
+
+    Args:
+        dcms (List[Dataset]): _description_
+        load_pixel_arr (bool, optional): _description_. Defaults to True.
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: _description_
+    """
     if load_pixel_arr:
         arr = load_as_arr(dcms)
     else:
         arr = None
     d0, d1, d2 = dcms[:3]
     s01 = abs(np.array(d0.ImagePositionPatient) - np.array(d1.ImagePositionPatient))
     s12 = abs(np.array(d1.ImagePositionPatient) - np.array(d2.ImagePositionPatient))
@@ -110,28 +142,50 @@
     assert x_spacing == y_spacing
     spacing = [x_spacing, y_spacing, z_spacing]
     affine = np.diag(spacing + [0])
     return affine, arr
 
 
 def load_as_arr(dcms: List[Dataset]) -> np.ndarray:
+    """
+    Load DICOM series as numpy array.
+    将DICOM序列加载为numpy矩阵。
+
+    Args:
+        dcms (List[Dataset]): _description_
+
+    Returns:
+        np.ndarray: _description_
+    """
     arr = []
     for d in dcms:
         # arr.append(np.rot90(d.pixel_array, 1, [0, 1]))
         arr.append(d.pixel_array)
     return np.stack(arr, axis=-1)
 
 
 def load_as_arr1(dcm_dir: os.PathLike) -> np.ndarray:
+    """
+    Same with load_as_arr but parameters.
+    除了参数，其它与load_as_arr一样。
+
+    Args:
+        dcm_dir (os.PathLike): _description_
+
+    Returns:
+        np.ndarray: _description_
+    """
     dcms = load_series(dcm_dir)
     return load_as_arr(dcms)
 
 
 def seg2arr(seg: Dataset) -> np.ndarray:
-    """seg转为arr，按照origin_dcm的顺序排列
+    """
+    Convert DICOM SEG to numpy array, and sort by the reference image.
+    DICOM SEG转为numpy数组，按照引用图像的顺序排列。
 
     Args:
         seg (Dataset): _description_
     """
     assert seg.Modality == 'SEG'
     # TODO 保证该SEG文件可以按照以下规则解析
 
@@ -150,15 +204,17 @@
         mask[:, :, index_][mask_frame==1] = segment_number
     return mask.astype(np.int8)
 
 
 def arr2seg(arr: np.ndarray, dicom: List[Dataset],
             series_description: str, save_path: os.PathLike = None,
             attributes: dict = {}, segment_label_map = {}) -> Dataset:
-    """将数组转为DICOM SEG文件
+    """
+    Convert array to DICOM SEG.
+    将数组转为DICOM SEG文件。
 
     Args:
         arr (np.ndarray): _description_
         dicom (List[Dataset]): 原始DICOM图像
         series_description (str): DICOM TAG SeriesDescription
         attributes (Dict): example: {"StudyDescription": "easy_tk_seg"}
         segment_label (Dict): example: {1: 'tumor1', 2: 'tumor2'}
@@ -497,15 +553,17 @@
         if key in ds_dir:
             setattr(d, key, value)
     return d
 
 
 def seg2nii(seg: Dataset, origin_dcm: List[Dataset], 
             save_path: os.PathLike=None) -> nib.Nifti1Image:
-    """convert DICOM SEG to NIfTI
+    """
+    Convert DICOM SEG to NIfTI.
+    DICOM SEG转为NIfTI.
 
     Args:
         seg (Dataset): _description_
         origin_dcm (List[Dataset]): _description_
         save_path (os.PathLike, optional): _description_. Defaults to None.
 
     Returns:
```

### Comparing `easy_mitk-0.0.1/easy_mitk/measure.py` & `easy_mitk-0.0.2/easy_mitk/measure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import vtk
 import nibabel as nib
 import numpy as np
 
 
 def volume(nii_path: os.PathLike):
-    """计算掩膜的体积 ml
+    """
+    计算掩膜的体积 (ml)
+    Compute volume of the mask (ml).
 
     Args:
         nii_path (os.PathLike): _description_
 
     Returns:
         _type_: _description_
     """
@@ -17,15 +19,17 @@
     pixdim = nii.header['pixdim']
     voxel_size = pixdim[1] * pixdim[2] * pixdim[3]
     arr = nii.get_fdata()
     count = np.count_nonzero(arr)
     return count * voxel_size / 1000
 
 def surface_area(nii_path: os.PathLike):
-    """计算掩膜的表面积 cm^2
+    """
+    计算掩膜的表面积 (cm^2)
+    Compute surface area of the mask (cm^2). 
 
     Args:
         nii_path (os.PathLike): _description_
 
     Returns:
         _type_: _description_
     """
```

### Comparing `easy_mitk-0.0.1/easy_mitk/utils/helper.py` & `easy_mitk-0.0.2/easy_mitk/utils/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 from typing import Tuple
 
 
 def bbox(data: np.ndarray) -> Tuple[slice]:
-    """返回一个数据的bounding box，这个数据通常是一个mask
+    """
+    Compute the max bounding box of a mask.
+    返回一个掩膜的最大边框。
 
     Args:
         data (np.ndarray): _description_
 
     Returns:
         Tuple[slice]: _description_
     """
```

### Comparing `easy_mitk-0.0.1/setup.py` & `easy_mitk-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="easy_mitk",
-    version="0.0.1",  # 本版本可以不进行更新
+    version="0.0.2",
     author="Daryl.Xu",
     author_email="ziqiang_xu@qq.com",
-    description="Easy medical imaging toolkit",
+    description="An easy-to-use Medical Imaging ToolKit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/daryl6/easy-mitk",
     packages=setuptools.find_packages(),
     install_requires=[
-        'pydicom', 'nibabel', 'pylibjpeg-rle', 'dicom2nifti'
+        'pydicom', 'nibabel', 'pylibjpeg-rle', 'dicom2nifti', 'numpy', 'vtk', 'pylibjpeg-rle'
         ],
     entry_points={
     },
     classifiers=(
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
     ),
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easy_mitk-0.0.1/tests/test_dicom.py` & `easy_mitk-0.0.2/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `easy_mitk-0.0.1/tests/test_measure.py` & `easy_mitk-0.0.2/tests/test_measure.py`

 * *Files identical despite different names*

