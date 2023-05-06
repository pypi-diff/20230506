# Comparing `tmp/dspawpy-0.9.1-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 70630 bytes, number of entries: 20
+Zip file size: 73004 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    29208 b- defN 23-Apr-25 05:34 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    24557 b- defN 23-Apr-29 05:39 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    24571 b- defN 23-May-06 03:20 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
 -rw-rw-rw-  2.0 fat     3592 b- defN 23-Apr-26 09:25 dspawpy/diffusion/neb.py
 -rw-rw-rw-  2.0 fat    53467 b- defN 23-Apr-26 09:25 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-Apr-25 05:34 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    48925 b- defN 23-Apr-29 02:43 dspawpy/io/read.py
+-rw-rw-rw-  2.0 fat    52393 b- defN 23-May-06 03:20 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-25 05:46 dspawpy/io/read_json.py
--rw-rw-rw-  2.0 fat     6163 b- defN 23-Apr-26 09:44 dspawpy/io/structure.py
+-rw-rw-rw-  2.0 fat     8538 b- defN 23-May-06 03:20 dspawpy/io/structure.py
 -rw-rw-rw-  2.0 fat    25241 b- defN 23-Apr-26 09:44 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    24416 b- defN 23-Apr-26 09:25 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat    28491 b- defN 23-May-06 03:20 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1761 b- defN 23-Apr-25 05:51 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     2036 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1581 b- defN 23-Apr-29 06:57 dspawpy-0.9.1.dist-info/RECORD
-20 files, 259965 bytes uncompressed, 68080 bytes compressed:  73.8%
+-rw-rw-rw-  2.0 fat     2215 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1581 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/RECORD
+20 files, 270076 bytes uncompressed, 70454 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.9.1.dist-info/METADATA
+Filename: dspawpy-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.1.dist-info/WHEEL
+Filename: dspawpy-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.1.dist-info/top_level.txt
+Filename: dspawpy-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.1.dist-info/RECORD
+Filename: dspawpy-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -128,23 +128,23 @@
 
         max_r = self.rmax + self.dr / 2.0  # add a small shell to improve robustness
 
         print(f"Calculating neighbor lists for {len(self.structures)} structures,")
         self.neighbor_lists = []
         for _c, i in enumerate(self.structures):
             if _c == 0:
-                print('0%...', end='', flush=True)
-            elif _c/len(self.structures)*100 == 25:
-                print('25%...', end='', flush=True)
-            elif _c/len(self.structures)*100 == 50:
-                print('50%...', end='', flush=True)
-            elif _c/len(self.structures)*100 == 75:
-                print('75%...', end='', flush=True)
-            elif _c == len(self.structures)-1:
-                print('100%')
+                print("0%...", end="", flush=True)
+            elif _c / len(self.structures) * 100 == 25:
+                print("25%...", end="", flush=True)
+            elif _c / len(self.structures) * 100 == 50:
+                print("50%...", end="", flush=True)
+            elif _c / len(self.structures) * 100 == 75:
+                print("75%...", end="", flush=True)
+            elif _c == len(self.structures) - 1:
+                print("100%")
             self.neighbor_lists.append(i.get_neighbor_list(max_r))
 
         # each neighbor list is a tuple of
         # center_indices, neighbor_indices, image_vectors, distances
         (
             self.center_indices,
             self.neighbor_indices,
```

## dspawpy/io/read.py

```diff
@@ -13,34 +13,42 @@
 from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 from pymatgen.electronic_structure.core import Orbital, Spin
 from pymatgen.electronic_structure.dos import CompleteDos, Dos
 from pymatgen.phonon.bandstructure import PhononBandStructureSymmLine
 from pymatgen.phonon.dos import PhononDos
 
 
-def get_band_data(band_dir: str, efermi: float = None) -> BandStructureSymmLine:
+def get_band_data(
+    band_dir: str, syst_dir: str = None, efermi: float = None
+) -> BandStructureSymmLine:
     """读取h5或json文件中的能带数据，构建BandStructureSymmLine对象
 
     Parameters
     ----------
     band_dir : str
         能带文件路径，band.h5 / band.json
+    syst_dir : str
+        system.json 路径，仅为辅助处理 Wannier 数据而准备
     efermi : float, optional
         费米能级，如果h5文件中的费米能级不正确，可以通过此参数指定费米能级
 
     Returns
     -------
     BandStructureSymmLine
 
     Examples
     --------
     >>> from dspawpy.io.read import get_band_data
     >>> band = get_band_data(band_dir='band.h5')
     >>> band.branches
     [{'start_index': 0, 'end_index': 100, 'name': 'R-G'}, {'start_index': 101, 'end_index': 201, 'name': 'G-X'}]
+
+    如果希望通过指定wannier.json来处理瓦尼尔能带，需要额外指定syst_dir参数
+
+    >>> band = get_band_data(band_dir='wannier.json', syst_dir='system.json')
     """
     if band_dir.endswith(".h5"):
         band = load_h5(band_dir)
         raw = h5py.File(band_dir, "r").keys()
         if "/WannBandInfo/NumberOfBand" in raw:
             (
                 structure,
@@ -62,22 +70,27 @@
         else:
             print("BandInfo or WannBandInfo key not found in h5file!")
             return
     elif band_dir.endswith(".json"):
         with open(band_dir, "r") as fin:
             band = json.load(fin)
         if "WannBandInfo" in band.keys():
+            assert (
+                syst_dir is not None
+            ), "system.json is required for processing wannier band info!"
+            with open(syst_dir) as system_json:
+                syst = json.load(system_json)
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
                 projections,
-            ) = _get_band_data_json(band, iwan=True)
+            ) = _get_band_data_json(band, syst, iwan=True)
         elif "BandInfo" in band.keys():
             (
                 structure,
                 kpoints,
                 eigenvals,
                 rEf,
                 labels_dict,
@@ -306,19 +319,19 @@
     """Wrapper to get structure information from h5/json/as file.
 
     从datafile中读取结构信息
 
     Parameters
     ----------
     datafile : str
-        h5 / json结果文件或as结构文件路径
+        h5 / json 文件路径
     scaled : bool, optional
         是否返回分数坐标，默认False
     index : int or list or str, optional
-        运动轨迹中的第几步，从1开始计数
+        运动轨迹中的第几步，从1开始计数！
         如果要切片，用字符串写法： '1, 10'
         默认为None，返回所有步
     ele : list, optional
         元素列表, Natom x 1
         默认为None，从h5文件中读取
     ai : int or list or str, optional
         多离子步中的第几个离子步，从1开始计数
@@ -341,41 +354,405 @@
     Examples
     --------
 
     >>> from dspawpy.io.read import get_sinfo
     >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='aimd.h5', scaled=False, index=None, ele=None, ai=None)
     >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='relax.json', scaled=False, index=None, ele=None, ai=None)
     >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='rho.json', scaled=False)
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='structure.as', scaled=False)
 
     这些信息可以用于进一步构建Structure对象，
     具体参考 dspawpy.io.structure.build_Structures_from_datafile 函数
+
     """
     if datafile.endswith(".h5"):
         assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
-        Nstep, eles, pos, latv, D_mag_fix = _sinfo_from_h5(
-            hpath=datafile, index=index, ele=ele, ai=ai, return_scaled=scaled
-        )
+        hpath = datafile
+        print(f"Reading {os.path.abspath(hpath)} ...")
+        hf = h5py.File(hpath)  # 加载h5文件
+
+        # decide task type by check the internal key
+        if "/Structures" in hf.keys():  # multi-steps
+            Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
+
+            if ele is not None and ai is not None:
+                raise ValueError("暂不支持同时指定元素和原子序号")
+            # 步数
+            if index is not None:
+                if isinstance(index, int):  # 1
+                    indices = [index]
+
+                elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = index
+
+                elif isinstance(index, str):  # ':', '-3:'
+                    indices = __parse_indices(index, Total_step)
+
+                else:
+                    raise ValueError("请输入正确格式的index")
+
+                Nstep = len(indices)
+            else:
+                Nstep = Total_step
+                indices = list(range(1, Nstep + 1))
+
+            # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
+            Elements = np.array(get_ele_from_h5(hpath), dtype=object)
+
+            # 开始读取晶胞和原子位置
+            lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
+            location = []
+            if ele is not None:  # 如果用户指定元素
+                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                    ele_list = np.array(ele, dtype=object)
+                    location = np.where(Elements == ele_list)[0]
+                # 多个元素符号组成的列表，例如 ['Fe', 'O']
+                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                    for e in ele:
+                        loc = np.where(Elements == e)[0]
+                        location.append(loc)
+                    location = np.concatenate(location)
+                else:
+                    raise TypeError("请输入正确的元素或元素列表")
+                elements = Elements[location]
+
+            elif ai is not None:  # 如果用户指定原子序号
+                if isinstance(ai, int):  # 1
+                    ais = [ai]
+                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    ais = ai
+                elif isinstance(ai, str):  # ':', '-3:'
+                    ais = __parse_indices(ai, Total_step)
+                else:
+                    raise ValueError("请输入正确格式的ai")
+                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+                elements = Elements[ais]
+                location = ais
+
+            else:  # 如果都没指定
+                elements = Elements
+                location = list(range(len(Elements)))
+
+            elements = elements.tolist()  # for pretty output
+            Natom = len(elements)
+            mags = []  # must be Nstep x Natom x ?
+
+            poses = np.empty(shape=(len(indices), Natom, 3))
+            wrapped_poses = np.empty(shape=(len(indices), 3, Natom))
+            for i, ind in enumerate(indices):  # 步数
+                # print(f'{ind=}')
+                lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
+                lattices[i] = lats
+                # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
+                # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
+                pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
+                wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
+                wrapped_pos = (
+                    wrapped_pos.flatten().reshape(-1, 3).T
+                )  # reshape to 3 x Natom
+                wrapped_poses[i] = wrapped_pos
+
+                iNoncollinear = False
+                try:  # 自旋计算
+                    if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
+                        mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
+                    elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
+                        magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
+                        magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
+                        magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
+                        iNoncollinear = True
+                    else:
+                        mag = np.zeros(shape=(Natom, 1))
+
+                except Exception as e:
+                    if str(e):  # ignore empty AssertionError()
+                        print(e)
+                    mag = np.zeros(shape=(Natom, 1))
+
+                mags.append(mag)
+
+            if "/AtomInfo/Fix" in hf.keys():  # fix atom
+                atomFixs_raw = np.array(hf.get("/AtomInfo/Fix"))
+                atomFixs = np.array(
+                    ["True" if _v else "False" for _v in atomFixs_raw]
+                ).reshape(-1, 3)
+            else:
+                atomFixs = np.full(shape=(Natom, 3), fill_value="False")
+
+            try:  # fix lattice
+                latticeFixs = (
+                    np.array(hf.get("/AtomInfo/FixLattice")).astype(bool).flatten()
+                )
+                assert latticeFixs.shape == (9,)
+                latticeFixs = latticeFixs.reshape(
+                    9,
+                )  # (9,)
+            except Exception as e:
+                if str(e):  # ignore empty AssertionError()
+                    print(e)
+                latticeFixs = np.full(shape=(9,), fill_value="False")
+
+            # repeat atomFixs of shape Natom x 3 to Nstep x Natom x 3
+            atomFixs = np.repeat(atomFixs[np.newaxis, :], Nstep, axis=0).reshape(
+                Nstep, Natom, 3
+            )
+
+            # repeat latticeFixs of shape 9 x 1 to Nstep x Natom x 9
+            latticeFixs = (
+                np.repeat(latticeFixs[np.newaxis, :], Nstep * Natom, axis=0)
+                .reshape(Nstep, Natom, 9)
+                .tolist()
+            )
+
+            if iNoncollinear == False:
+                mags = np.array(mags).reshape(Nstep, Natom, -1).tolist()
+                D_mag_fix = {
+                    "Mag": mags,
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+            else:
+                D_mag_fix = {
+                    "Mag_x": magx,
+                    "Mag_y": magy,
+                    "Mag_z": magz,
+                    "Fix_x": atomFixs[:, :, 0],
+                    "Fix_y": atomFixs[:, :, 1],
+                    "Fix_z": atomFixs[:, :, 2],
+                    "LatticeFixs": latticeFixs,
+                }
+
+            if scaled:  # Fractional coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):  # atom index
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
+            else:  # Cartesian coordinates
+                for k, ind in enumerate(indices):  # 步数
+                    for j, sli in enumerate(location):
+                        poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
+
+        elif "/UnrelaxStructure" in hf.keys():  # single-step
+            raise NotImplementedError(
+                "Read from neb.h5 is not implemented yet!\n you may try neb01.h5.."
+            )
+        elif "/UnitAtomInfo" in hf.keys():  # phonon
+            raise NotImplementedError(
+                "Read from phonon.h5 is not implemented yet!\n you may try phonon001.h5.."
+            )
+        else:  # rho, potential, elf, pcharge
+            hfDict = load_h5(hpath)
+            s = _get_structure(hfDict, "/AtomInfo")
+            elements = s.species
+            poses = [s.cart_coords]
+            lattices = [s.lattice.matrix]
+            Nstep = 1
+            D_mag_fix = None
+            print("--> rho/potential/elf/pcharge.h5 has no mag or fix info,")
+            print("  you should manually set it before starting new calculations..")
+
     elif datafile.endswith(".json"):
         assert os.path.exists(datafile), f"{os.path.abspath(datafile)} does not exist!"
-        Nstep, eles, pos, latv, D_mag_fix = _sinfo_from_json(
-            jpath=datafile, index=index, ele=ele, ai=ai, return_scaled=scaled
-        )
-    elif datafile.endswith(".as"):
-        print("Reading mag & fix info from .as file is not supported yet!")
-        p, e, l = pel_from_as(spath=datafile, scaled=scaled)
-        pos = [p]
-        eles = e
-        latv = [l]
-        Nstep = 1
-        D_mag_fix = None
+        jpath = datafile
+        print(f"Reading {os.path.abspath(jpath)}...")
+        with open(jpath, "r") as f:
+            data = json.load(f)  # 加载json文件
+
+        # decide the task type by checking the internal keys
+        if "AtomInfo" in data:  # single-step task
+            s = _get_structure_json(data["AtomInfo"])
+            elements = s.species
+            poses = [s.cart_coords]
+            lattices = [s.lattice.matrix]
+            Nstep = 1
+            D_mag_fix = None
+
+        elif "UnitAtomInfo" in data:  # phonon task
+            raise NotImplementedError("Read from phonon.json is not supported yet.")
+        elif "IniFin" in data:  # neb.json
+            raise NotImplementedError("Read from neb.json is not supported yet.")
+        elif "WannierInfo" in data:
+            raise NotImplementedError("wannier.json has no stucture info!")
+
+        else:  # multi-steps task
+            if "Structures" in data:
+                Total_step = len(data["Structures"])  # aimd.json
+            else:
+                Total_step = len(data)  # relax.json, neb01.json
+
+            if ele is not None and ai is not None:
+                raise ValueError("暂不支持同时指定元素和原子序号")
+            # 步数
+            if index is not None:
+                if isinstance(index, int):  # 1
+                    indices = [index]
+
+                elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = index
+
+                elif isinstance(index, str):  # ':', '-3:'
+                    indices = __parse_indices(index, Total_step)
+
+                else:
+                    raise ValueError("请输入正确格式的index")
+
+                Nstep = len(indices)
+            else:
+                Nstep = Total_step
+                indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
+
+            # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
+            # 这样可以避免在循环内部频繁判断元素是否符合用户需要
+
+            if "Structures" in data:
+                Nele = len(data["Structures"][0]["Atoms"])  # relax.json
+                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+                for i in range(Nele):
+                    element = data["Structures"][0]["Atoms"][i]["Element"]
+                    total_elements[i] = element
+            else:
+                if "Atoms" not in data[0]:
+                    raise NotImplementedError("nebXX.json has no structure info!")
+                Nele = len(data[0]["Atoms"])
+                total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
+                for i in range(Nele):
+                    element = data[0]["Atoms"][i]["Element"]
+                    total_elements[i] = element
+
+            Natom = len(total_elements)
+
+            # 开始读取晶胞和原子位置
+            # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
+            if ele is not None:  # 用户指定要某些元素
+                location = []
+                if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
+                    ele_list = list(ele)
+                # 多个元素符号组成的列表，例如 ['Fe', 'O']
+                elif isinstance(ele, list) or isinstance(ele, np.ndarray):
+                    ele_list = ele
+                else:
+                    raise TypeError("请输入正确的元素或元素列表")
+                for e in ele_list:
+                    location.append(np.where(total_elements == e)[0])
+                location = np.concatenate(location)
+
+            elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
+                if isinstance(ai, int):  # 1
+                    ais = [ai]
+                elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    ais = ai
+                elif isinstance(ai, str):  # ':', '-3:'
+                    ais = __parse_indices(ai, Total_step)
+                else:
+                    raise ValueError("请输入正确格式的ai")
+                ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
+                location = ais
+                # read lattices and poses
+
+            else:  # 如果都没指定
+                location = list(range(Natom))
+
+            # 满足用户需要的elements列表
+            elements = np.empty(shape=(Natom,), dtype=object)
+            for i in range(len(location)):
+                elements[i] = total_elements[location[i]]
+
+            # Nstep x Natom x 3, positions are all fractional
+            poses = np.empty(shape=(len(indices), len(elements), 3))
+            lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
+            mags = []  # Nstep x Natom x ?
+            Atomfixs = []  # Nstep x Natom x 1
+            LatFixs = []  # Nstep x Natom x 9
+
+            if "Structures" in data:  # aimd
+                for i, ind in enumerate(indices):  # for every ionic step
+                    lat = data["Structures"][ind - 1]["Lattice"]
+                    lattices[i] = np.array(lat).reshape(3, 3)
+                    mag_for_each_step = []
+                    fix_for_each_step = []
+                    fixlat_raw = data["Structures"][ind - 1]["FixLattice"]
+                    if fixlat_raw == []:
+                        fixlat_raw = np.full((9, 1), fill_value=False).tolist()
+                    fixlat_str = [
+                        "True" if _v == True else "False" for _v in fixlat_raw
+                    ]
+                    fixlat_arr = np.array(fixlat_str).reshape(9, 1)
+                    # repeat fixlat for each atom
+                    fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
+                    LatFixs.append(fixlat)
+                    for j, sli in enumerate(location):
+                        ati = data["Structures"][ind - 1]["Atoms"][sli]
+                        poses[i, j, :] = ati["Position"][:]
+
+                        mag_for_each_atom = ati["Mag"][:]
+                        if mag_for_each_atom == []:
+                            mag_for_each_atom = [0.0]
+                        mag_for_each_step.append(mag_for_each_atom)
+
+                        fix_for_each_atom = ati["Fix"][:]
+                        if fix_for_each_atom == []:
+                            fix_for_each_atom = ["False"]
+                        fix_for_each_step.append(fix_for_each_atom)
+
+                    mags.append(mag_for_each_step)
+                    Atomfixs.append(fix_for_each_step)
+                    if not scaled:
+                        poses = np.dot(poses, lattices[i])
+
+            else:  # relax, neb01
+                print(
+                    "Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info..."
+                )
+
+                for i, ind in enumerate(indices):  # for every ionic step
+                    lat = data[ind - 1]["Lattice"]
+                    lattices[i] = np.array(lat).reshape(3, 3)
+                    mag_for_each_step = []
+                    fix_for_each_step = []
+                    fixlat_raw = data[ind - 1]["FixLattice"]
+                    if fixlat_raw == None:
+                        fixlat_raw = np.full((9, 1), fill_value=False).tolist()
+                    fixlat_str = [
+                        "True" if _v == True else "False" for _v in fixlat_raw
+                    ]
+                    fixlat_arr = np.array(fixlat_str).reshape(9, 1)
+                    # repeat fixlat for each atom
+                    fixlat = np.repeat(fixlat_arr, Natom, axis=1).T.tolist()
+                    LatFixs.append(fixlat)
+
+                    for j, sli in enumerate(location):
+                        ati = data[ind - 1]["Atoms"][sli]
+                        poses[i, j, :] = ati["Position"][:]
+
+                        mag_for_each_atom = ati["Mag"][:]
+                        if mag_for_each_atom == []:
+                            mag_for_each_atom = [0.0]
+                        mag_for_each_step.append(mag_for_each_atom)
+
+                        fix_for_each_atom = ati["Fix"][:]
+                        if fix_for_each_atom == []:
+                            fix_for_each_atom = ["False"]
+                        fix_for_each_step.append(fix_for_each_atom)
+
+                    mags.append(mag_for_each_step)
+                    Atomfixs.append(fix_for_each_step)
+                    if not scaled:
+                        poses = np.dot(poses, lattices[i])
+
+            elements = elements.tolist()
+            Mags = np.array(mags).tolist()  # (Nstep, Natom, ?) or (Nstep, 0,)
+
+            D_mag_fix = {"Mag": Mags, "Fix": Atomfixs, "LatticeFixs": LatFixs}
+
     else:
-        raise ValueError("datafile must be .h5 / .json / .as file!")
+        raise ValueError(
+            "get_sinfo function only accept datafile of .h5 / .json format!"
+        )
 
-    return Nstep, eles, pos, latv, D_mag_fix
+    return Nstep, elements, poses, lattices, D_mag_fix
 
 
 def pel_from_as(spath: str, scaled=False):
     """Extract structure information from .as file
 
     从DSPAW的as结构文件中读取坐标、元素列表，和晶胞信息
 
@@ -530,347 +907,14 @@
     groups_value_dict = {}
     for data in groups_value_list:
         create_dict(data, groups_value_dict)
 
     return groups_value_dict
 
 
-def _sinfo_from_h5(
-    hpath: str,
-    index=None,
-    ele=None,
-    ai=None,
-    return_scaled: bool = False,
-):
-    print(f"Reading {os.path.abspath(hpath)} ...")
-    hf = h5py.File(hpath)  # 加载h5文件
-
-    # decide task type by check the internal key
-    if "/Structures" in hf.keys():  # multi-steps
-        Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
-
-        if ele is not None and ai is not None:
-            raise ValueError("暂不支持同时指定元素和原子序号")
-        # 步数
-        if index is not None:
-            if isinstance(index, int):  # 1
-                indices = [index]
-
-            elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                indices = index
-
-            elif isinstance(index, str):  # ':', '-3:'
-                indices = __parse_indices(index, Total_step)
-
-            else:
-                raise ValueError("请输入正确格式的index")
-
-            Nstep = len(indices)
-        else:
-            Nstep = Total_step
-            indices = list(range(1, Nstep + 1))
-
-        # 读取元素列表，这个列表不会随步数改变，也不会“合并同类项”
-        Elements = np.array(get_ele_from_h5(hpath), dtype=object)
-
-        # 开始读取晶胞和原子位置
-        lattices = np.empty((Nstep, 3, 3))  # Nstep x 3 x 3
-        location = []
-        if ele is not None:  # 如果用户指定元素
-            if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-                ele_list = np.array(ele, dtype=object)
-                location = np.where(Elements == ele_list)[0]
-            # 多个元素符号组成的列表，例如 ['Fe', 'O']
-            elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-                for e in ele:
-                    loc = np.where(Elements == e)[0]
-                    location.append(loc)
-                location = np.concatenate(location)
-            else:
-                raise TypeError("请输入正确的元素或元素列表")
-            elements = Elements[location]
-
-        elif ai is not None:  # 如果用户指定原子序号
-            if isinstance(ai, int):  # 1
-                ais = [ai]
-            elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                ais = ai
-            elif isinstance(ai, str):  # ':', '-3:'
-                ais = __parse_indices(ai, Total_step)
-            else:
-                raise ValueError("请输入正确格式的ai")
-            ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-            elements = Elements[ais]
-            location = ais
-
-        else:  # 如果都没指定
-            elements = Elements
-            location = list(range(len(Elements)))
-
-        elements = elements.tolist()  # for pretty output
-
-        mags = []  # must be Nstep x Natom x ?
-
-        poses = np.empty(shape=(len(indices), len(elements), 3))
-        wrapped_poses = np.empty(shape=(len(indices), 3, len(elements)))
-        for i, ind in enumerate(indices):  # 步数
-            # print(f'{ind=}')
-            lats = np.array(hf.get("/Structures/Step-" + str(ind) + "/Lattice"))
-            lattices[i] = lats
-            # [x1,y1,z1,x2,y2,z2,x3,y3,z3], ...
-            # 结构优化时输出的都是分数坐标，不管CoordinateType写的是啥！
-            pos = np.array(hf.get("/Structures/Step-" + str(ind) + "/Position"))
-            wrapped_pos = pos - np.floor(pos)  # wrap into [0,1)
-            wrapped_pos = wrapped_pos.flatten().reshape(-1, 3).T  # reshape to 3 x Natom
-            wrapped_poses[i] = wrapped_pos
-
-            try:  # 自旋计算
-                mag = np.array(hf.get("/Structures/Step-" + str(ind) + "/Mag"))
-                if mag == None:
-                    mag = np.zeros(shape=(len(elements), 1))
-            except Exception as e:
-                if str(e): # ignore empty AssertionError()
-                    print(e)
-                mag = np.zeros(shape=(len(elements), 1))
-            mags.append(mag)
-
-        try:  # fix atom
-            atomfixs = np.array(hf.get("/AtomInfo/Fix")).astype(bool).flatten()
-            assert atomfixs.shape == (12,)  # np.ndarray (Natom x 3, )
-            atomfixs = atomfixs.reshape(-1, 3)  # (Natom, 3)
-        except Exception as e:
-            if str(e): # ignore empty AssertionError()
-                print(e)
-            atomfixs = np.full(shape=(len(elements), 3), fill_value=False)
-
-        mags = np.array(mags).reshape(Nstep, len(elements), -1)
-        # repeat atomfixs to Nstep x Natom x 3
-        atomfixs = np.repeat(atomfixs[np.newaxis, :, :], Nstep, axis=0).tolist()
-
-        D_mag_fix = {"Mags": mags, "AtomFixs": atomfixs}
-
-        if return_scaled:  # Fractional coordinates
-            for k, ind in enumerate(indices):  # 步数
-                for j, sli in enumerate(location):  # atom index
-                    poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
-        else:  # Cartesian coordinates
-            for k, ind in enumerate(indices):  # 步数
-                for j, sli in enumerate(location):
-                    poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
-
-        return Nstep, elements, poses, lattices, D_mag_fix
-
-    elif "/UnrelaxStructure" in hf.keys():  # single-step
-        raise NotImplementedError(
-            "Read from neb.h5 is not implemented yet!\n you may try neb01.h5.."
-        )
-    elif "/UnitAtomInfo" in hf.keys():  # phonon
-        raise NotImplementedError(
-            "Read from phonon.h5 is not implemented yet!\n you may try phonon001.h5.."
-        )
-    else:  # rho, potential, elf, pcharge
-        hfDict = load_h5(hpath)
-        s = _get_structure(hfDict, "/AtomInfo")
-        elements = s.species
-        poses = [s.cart_coords]
-        lattices = [s.lattice.matrix]
-        Nstep = 1
-        D_mag_fix = None
-        # print(
-        #     "You should check lattice fix info and manually set it before starting new calculations.."
-        # )
-
-        return Nstep, elements, poses, lattices, D_mag_fix
-
-
-def _sinfo_from_json(
-    jpath: str,
-    index=None,
-    ele=None,
-    ai=None,
-    return_scaled=False,
-):
-    """从json指定的路径读取结构相关数据
-
-    输入:
-    - jpath: json文件路径
-    - ai: 原子序号（体系中的第几个原子，不是质子数）
-    - ele: 元素，例如 'C'，'H'，'O'，'N'
-    - index: 运动轨迹中的第几步，从1开始
-
-    输出：
-    - Nstep: 总共要保存多少步的信息, int
-    - elements: 元素列表, list, Natom x 1
-    - positions: 原子位置, list, Nstep x Natom x 3
-    - lattices: 晶胞, list, Nstep x 3 x 3
-    """
-    print(f"Reading {os.path.abspath(jpath)}...")
-    with open(jpath, "r") as f:
-        data = json.load(f)  # 加载json文件
-
-    # decide the task type by checking the internal keys
-    if "AtomInfo" in data:  # single-step task
-        s = _get_structure_json(data["AtomInfo"])
-        elements = s.species
-        poses = [s.cart_coords]
-        lattices = [s.lattice.matrix]
-        Nstep = 1
-        D_mag_fix = None
-        return Nstep, elements, poses, lattices, D_mag_fix
-
-    elif "UnitAtomInfo" in data:  # phonon task
-        raise NotImplementedError("Read from phonon.json is not supported yet.")
-    elif "IniFin" in data:  # neb.json
-        raise NotImplementedError("Read from neb.json is not supported yet.")
-    elif "WannierInfo" in data:
-        raise NotImplementedError("wannier.json has no stucture info!")
-    else:  # multi-steps task
-        if "Structures" in data:
-            Total_step = len(data["Structures"])  # aimd.json
-        else:
-            Total_step = len(data)  # relax.json, neb01.json
-
-        if ele is not None and ai is not None:
-            raise ValueError("暂不支持同时指定元素和原子序号")
-        # 步数
-        if index is not None:
-            if isinstance(index, int):  # 1
-                indices = [index]
-
-            elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                indices = index
-
-            elif isinstance(index, str):  # ':', '-3:'
-                indices = __parse_indices(index, Total_step)
-
-            else:
-                raise ValueError("请输入正确格式的index")
-
-            Nstep = len(indices)
-        else:
-            Nstep = Total_step
-            indices = list(range(1, Nstep + 1))  # [1,Nstep+1)
-
-        # 预先读取全部元素的总列表，这个列表不会随步数改变，也不会“合并同类项”
-        # 这样可以避免在循环内部频繁判断元素是否符合用户需要
-
-        if "Structures" in data:
-            Nele = len(data["Structures"][0]["Atoms"])  # relax.json
-            total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-            for i in range(Nele):
-                element = data["Structures"][0]["Atoms"][i]["Element"]
-                total_elements[i] = element
-        else:
-            if "Atoms" not in data[0]:
-                raise NotImplementedError("nebXX.json has no structure info!")
-            Nele = len(data[0]["Atoms"])
-            total_elements = np.empty(shape=(Nele), dtype=object)  # 未合并的元素列表
-            for i in range(Nele):
-                element = data[0]["Atoms"][i]["Element"]
-                total_elements[i] = element
-
-        Natom = len(total_elements)
-
-        # 开始读取晶胞和原子位置
-        # 在data['Structures']['%d' % index]['Atoms']中根据元素所在序号选择结构
-        if ele is not None:  # 用户指定要某些元素
-            location = []
-            if isinstance(ele, str):  # 单个元素符号，例如 'Fe'
-                ele_list = list(ele)
-            # 多个元素符号组成的列表，例如 ['Fe', 'O']
-            elif isinstance(ele, list) or isinstance(ele, np.ndarray):
-                ele_list = ele
-            else:
-                raise TypeError("请输入正确的元素或元素列表")
-            for e in ele_list:
-                location.append(np.where(total_elements == e)[0])
-            location = np.concatenate(location)
-
-        elif ai is not None:  # 如果用户指定原子序号，也要据此筛选元素列表
-            if isinstance(ai, int):  # 1
-                ais = [ai]
-            elif isinstance(ai, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                ais = ai
-            elif isinstance(ai, str):  # ':', '-3:'
-                ais = __parse_indices(ai, Total_step)
-            else:
-                raise ValueError("请输入正确格式的ai")
-            ais = [i - 1 for i in ais]  # python从0开始计数，但是用户从1开始计数
-            location = ais
-            # read lattices and poses
-
-        else:  # 如果都没指定
-            location = list(range(Natom))
-
-        # 满足用户需要的elements列表
-        elements = np.empty(shape=(Natom,), dtype=object)
-        for i in range(len(location)):
-            elements[i] = total_elements[location[i]]
-
-        # Nstep x Natom x 3, positions are all fractional
-        positions = np.empty(shape=(len(indices), len(elements), 3))
-        lattices = np.empty(shape=(Nstep, 3, 3))  # Nstep x 3 x 3
-        mags = []  # Nstep x Natom x ?
-        Atomfixs = []  # Nstep x Natom x 3
-
-        if "Structures" in data:  # relax.json
-            for i, ind in enumerate(indices):  # for every ionic step
-                lat = data["Structures"][ind - 1]["Lattice"]
-                lattices[i] = np.array(lat).reshape(3, 3)
-                mag_for_each_step = []
-                fix_for_each_step = []
-                for j, sli in enumerate(location):
-                    ati = data["Structures"][ind - 1]["Atoms"][sli]
-                    positions[i, j, :] = ati["Position"][:]
-
-                    mag_for_each_atom = ati["Mag"][:]
-                    mag_for_each_step.append(mag_for_each_atom)
-
-                    fix_for_each_atom = ati["Fix"][:]
-                    if fix_for_each_atom == []:
-                        fix_for_each_atom = [0, 0, 0]
-                    fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
-                    fix_for_each_step.append(fix_for_each_atom)
-
-                mags.append(mag_for_each_step)
-                Atomfixs.append(fix_for_each_step)
-                if not return_scaled:
-                    positions = np.dot(positions, lattices[i])
-        else:
-            for i, ind in enumerate(indices):  # for every ionic step
-                lat = data[ind - 1]["Lattice"]
-                lattices[i] = np.array(lat).reshape(3, 3)
-                mag_for_each_step = []
-                fix_for_each_step = []
-                for j, sli in enumerate(location):
-                    ati = data[ind - 1]["Atoms"][sli]
-                    positions[i, j, :] = ati["Position"][:]
-
-                    mag_for_each_atom = ati["Mag"][:]
-                    mag_for_each_step.append(mag_for_each_atom)
-
-                    fix_for_each_atom = ati["Fix"][:]
-                    if fix_for_each_atom == []:
-                        fix_for_each_atom = [0, 0, 0]
-                    fix_for_each_atom = [bool(i) for i in fix_for_each_atom]
-                    fix_for_each_step.append(fix_for_each_atom)
-
-                mags.append(mag_for_each_step)
-                Atomfixs.append(fix_for_each_step)
-                if not return_scaled:
-                    positions = np.dot(positions, lattices[i])
-
-        elements = elements.tolist()
-        Mags = np.array(mags)  # (Nstep, Natom, ?) or (Nstep, 0,)
-
-        D_mag_fix = {"Mags": Mags, "AtomFixs": Atomfixs}
-
-        return Nstep, elements, positions, lattices, D_mag_fix
-
-
 def __parse_indices(index: str, total_step) -> list:
     """解析用户输入的原子序号字符串
 
     输入：
         - index: 用户输入的原子序号/元素字符串，例如 '1:3,5,7:10'
     输出：
         - indices: 解析后的原子序号列表，例如 [1,2,3,4,5,6,7,8,9,10]
@@ -1183,19 +1227,22 @@
                             .T
                         )
                 projections[spin] = projection
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
-def _get_band_data_json(band: dict, iwan=False):
+def _get_band_data_json(band: dict, syst: dict = None, iwan=False):
+    # syst is only required for wannier band structure
     if iwan:
         bd = "WannBandInfo"
+        structure = _get_structure_json(syst["AtomInfo"])
     else:
         bd = "BandInfo"
+        structure = _get_structure_json(band["AtomInfo"])
 
     number_of_band = band[f"{bd}"]["NumberOfBand"]
     number_of_kpoints = band[f"{bd}"]["NumberOfKpoints"]
     if "Spin2" in band[f"{bd}"]:
         number_of_spin = 2
     else:
         number_of_spin = 1
@@ -1224,15 +1271,14 @@
 
         eigenvals[spin] = band_data
 
     kpoints = np.asarray(band[f"{bd}"]["CoordinatesOfKPoints"]).reshape(
         number_of_kpoints, 3
     )
 
-    structure = _get_structure_json(band["AtomInfo"])
     labels_dict = {}
 
     for i, s in enumerate(band[f"{bd}"]["SymmetryKPoints"]):
         labels_dict[s] = kpoints[symmetry_kPoints_index[i] - 1]
 
     # read projection data
     projections = None
```

## dspawpy/io/structure.py

```diff
@@ -6,33 +6,33 @@
 
 import numpy as np
 from pymatgen.core import Structure
 
 from dspawpy.io.read import get_lines_without_comment, get_sinfo
 
 
-def build_Structures_from_datafile(datafile: Union[str, List[str]]) -> List[Structure]:
+def build_Structures_from_datafile(
+    datafile: Union[str, List[str]], scaled=False, index=None, ele=None, ai=None
+) -> List[Structure]:
     """读取一/多个h5/json文件，返回pymatgen的Structures列表
 
     Parameters
     ----------
     datafile : 字符串或字符串列表
-        aimd.h5/aimd.json文件或包含任意这些文件文件夹；若给定字符串列表，将依次读取数据并合并成一个Structures列表
+        h5/json/as/hzw文件路径；若给定字符串列表，将依次读取数据并合并成一个Structures列表
 
     Returns
     -------
     List[Structure] : pymatgen structures 列表
 
     Examples
     --------
-    >>> from dspawpy.analysis.aimdtools import build_Structures_from_datafile
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
     # 读取单个文件
     >>> pymatgen_Structures = build_Structures_from_datafile(datafile='aimd1.h5')
-    # 给定包含aimd.h5或aimd.json文件的文件夹位置
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='my_aimd_task')
     # 当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
     >>> pymatgen_Structures = build_Structures_from_datafile(datafile=['aimd1.h5','aimd2.h5'])
     """
     dfs = []
     if isinstance(datafile, list):  # 续算模式，给的是多个文件
         dfs = datafile
     else:  # 单次计算模式，处理单个文件
@@ -45,64 +45,76 @@
         else:
             raise FileNotFoundError("未找到h5或json文件！")
         dfs.append(df)
 
     # 读取结构数据
     pymatgen_Structures = []
     for df in dfs:
-        structure_list = _get_structure_list(df)
+        structure_list = _get_structure_list(df, scaled, index, ele, ai)
         pymatgen_Structures.extend(structure_list)
 
     return pymatgen_Structures
 
 
-def _get_structure_list(df: str = "aimd.h5") -> List[Structure]:
+def _get_structure_list(
+    df: str, scaled=False, index=None, ele=None, ai=None
+) -> List[Structure]:
     """get pymatgen structures from single datafile
 
     Parameters
     ----------
-    df : str, optional
-        datafile, by default "aimd.h5"
+    df : str
+        datafile
 
     Returns
     -------
     List[Structure] : list of pymatgen structures
 
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_structure_list
     >>> structure_list = get_structure_list(df='aimd.h5')
     """
 
     # create Structure structure_list from aimd.h5
-    Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(df)
-    strs = []
-    for i in range(Nstep):
-        if D_mag_fix:
-            strs.append(
-                Structure(
-                    lattices[i],
-                    elements,
-                    positions[i],
-                    coords_are_cartesian=False,
-                    site_properties={
-                        "Mags": D_mag_fix["Mags"][i],
-                        "AtomFixs": D_mag_fix["AtomFixs"][i],
-                    },
+    if df.endswith(".as"):
+        strs = [_from_dspaw_as(df)]
+    elif df.endswith(".hzw"):
+        print("build from hzw file may lack mag & fix info!")
+        strs = [_from_hzw(df)]
+    else:
+        assert df.endswith(".h5") or df.endswith(
+            ".json"
+        ), "datafile must be h5/json/as/hzw file!"
+
+        Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
+            df, scaled, index, ele, ai
+        )
+        icart = 0 if scaled else 1  # 0: scaled, 1: cartesian
+        strs = []
+        for i in range(Nstep):
+            if D_mag_fix:
+                strs.append(
+                    Structure(
+                        lattices[i],
+                        elements,
+                        positions[i],
+                        coords_are_cartesian=icart,
+                        site_properties={k: v[i] for k, v in D_mag_fix.items()},
+                    )
                 )
-            )
-        else:
-            strs.append(
-                Structure(
-                    lattices[i],
-                    elements,
-                    positions[i],
-                    coords_are_cartesian=False,
+            else:
+                strs.append(
+                    Structure(
+                        lattices[i],
+                        elements,
+                        positions[i],
+                        coords_are_cartesian=icart,
+                    )
                 )
-            )
     return strs
 
 
 def _from_dspaw_as(as_file: str = "structure.as") -> Structure:
     """从DSPAW的as结构文件中读取结构信息
 
     Parameters
@@ -116,54 +128,109 @@
         pymatgen的Structure对象
 
     Examples
     --------
     >>> from dspawpy.io.structure import from_dspaw_as
     >>> S1 = from_dspaw_as(as_file='structure00.as')
     """
-    D = {}
+
     lines = get_lines_without_comment(as_file, "#")
-    N = int(lines[1])
-    lattice = []
+    N = int(lines[1])  # number of atoms
+
+    # parse lattice info
+    lattice = []  # lattice matrix
     for line in lines[3:6]:
         vector = line.split()
         lattice.extend([float(vector[0]), float(vector[1]), float(vector[2])])
-
     lattice = np.asarray(lattice).reshape(3, 3)
-    is_direct = lines[6].strip().split()[0].startswith("Direct")
+
+    lat_fixs = []
+    if lines[2].strip() != "Lattice":  # fix lattice
+        lattice_fix_info = lines[2].strip().split()[1:]
+        if lattice_fix_info == ["Fix_x", "Fix_y", "Fix_z"]:
+            # ONLY support xyz fix in sequence, yzx will cause error
+            for line in lines[3:6]:
+                lfs = line.strip().split()[3:6]
+                for lf in lfs:
+                    if lf.startswith("T"):
+                        lat_fixs.append("True")
+                    elif lf.startswith("F"):
+                        lat_fixs.append("False")
+        elif lattice_fix_info == ["Fix"]:
+            for line in lines[3:6]:
+                lf = line.strip().split()[3]
+                if lf.startswith("T"):
+                    lat_fixs.append("True")
+                elif lf.startswith("F"):
+                    lat_fixs.append("False")
+        else:
+            raise ValueError("Lattice fix info error!")
+
     elements = []
     positions = []
-    others = []
-    line6s = []  # Cartesian/Direct Mag Fix_x ...
     for i in range(N):
         atom = lines[i + 7].strip().split()
         elements.append(atom[0])
         positions.extend([float(atom[1]), float(atom[2]), float(atom[3])])
 
-        if len(atom) > 4:
-            other = atom[4:]
-            others.append(other)
-            line6 = lines[6]
-            line6s.append(line6)
-
-    D.setdefault("others", others)
-    D.setdefault("line6s", line6s)
+    mf_info = None
+    l6 = lines[6].strip()  # str, 'Cartesian/Direct Mag Fix_x ...'
+    if l6 == "Direct":
+        is_direct = True
+    elif l6 == "Cartesian":
+        is_direct = False
+    else:
+        is_direct = l6.split()[0] == "Direct"
+        mf_info = l6.split()[1:]  # ['Mag', 'Fix_x', 'Fix_y', 'Fix_z']
+        for item in mf_info:
+            assert item in [
+                "Mag",
+                "Mag_x",
+                "Mag_y",
+                "Mag_z",
+                "Fix",
+                "Fix_x",
+                "Fix_y",
+                "Fix_z",
+            ], "Mag/Fix info error!"
+
+    mag_fix_dict = {}
+    if mf_info is not None:
+        for mf_index, item in enumerate(mf_info):
+            values = []
+            for i in range(N):
+                atom = lines[i + 7].strip().split()
+                mf = atom[4:]
+                values.append(mf[mf_index])
+
+            if item.startswith("Fix"):  # F -> False, T -> True
+                for value in values:
+                    if value.startswith("T"):
+                        values[values.index(value)] = "True"
+                    elif value.startswith("F"):
+                        values[values.index(value)] = "False"
+            mag_fix_dict[item] = values
+
+    if lat_fixs != []:
+        # replicate lat_fixs to N atoms
+        mag_fix_dict["LatticeFixs"] = [lat_fixs for i in range(N)]
 
     coords = np.asarray(positions).reshape(-1, 3)
-    if others == [] and line6s == []:
+
+    if mag_fix_dict == {}:
         return Structure(
             lattice, elements, coords, coords_are_cartesian=(not is_direct)
         )
     else:
         return Structure(
             lattice,
             elements,
             coords,
             coords_are_cartesian=(not is_direct),
-            site_properties=D,
+            site_properties=mag_fix_dict,
         )
 
 
 def _from_hzw(hzw_file) -> Structure:
     """从hzw结构文件中读取结构信息
 
     Parameters
```

## dspawpy/io/write.py

```diff
@@ -3,27 +3,26 @@
 """
 
 import json
 import os
 
 import numpy as np
 
-from dspawpy.io.read import (_get_lammps_non_orthogonal_box, _sinfo_from_h5,
-                             _sinfo_from_json, load_h5)
+from dspawpy.io.read import _get_lammps_non_orthogonal_box, get_sinfo, load_h5
 
 
 def write_xyz_traj(
     datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     xyzfile="aimdTraj.xyz",
     icombine=False,
 ):
-    """保存xyz格式的轨迹文件
+    r"""保存xyz格式的轨迹文件
 
     Parameters
     ----------
     datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
@@ -34,16 +33,17 @@
     xyzfile : str
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
     icombine : bool
         是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
-    >>> from dspawpy.analysis.write import write_xyz_traj
+    >>> from dspawpy.io.write import write_xyz_traj
     >>> write_xyz_traj(datafile='aimd.h5', ai=[1,2,3], index=1, xyzfile='aimdTraj.xyz')
+    Reading E:\Dev\dspawpy\test\new\aimd.h5 ...
     """
     if isinstance(datafile, list):
         dfs = datafile
     elif isinstance(datafile, str):
         dfs = [datafile]
     else:
         raise TypeError("datafile must be a str or a list of str!")
@@ -65,22 +65,20 @@
                 print("Reading aimd.h5...")
             elif os.path.exists(os.path.join(directory, "aimd.json")):
                 df = os.path.join(directory, "aimd.json")
                 print("Reading aimd.json...")
             else:
                 raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
 
-        if df.endswith(".h5"):
-            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_h5(
-                df, index, ele, ai, return_scaled=True
+        if df.endswith(".h5") or df.endswith(".json"):
+            Nstep, eles, poses, lats, D_mag_fix = get_sinfo(
+                datafile=df, scaled=True, index=index, ele=ele, ai=ai
             )
-        elif df.endswith(".json"):
-            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_json(df, index, ele, ai)
         else:
-            raise TypeError("仅支持读取h5或json文件！")
+            raise TypeError("write_xyz_traj 仅支持读取h5或json文件！")
 
         # 写入文件
         with open(xyzfilename, "w") as f:
             # Nstep
             for n in range(Nstep):
                 # 原子数不会变，就是不合并的元素总数
                 f.write("%d\n" % len(eles))
@@ -123,15 +121,15 @@
     datafile="aimd.h5",
     ai=None,
     ele=None,
     index=None,
     dumpfile="aimdTraj.dump",
     icombine=False,
 ):
-    """保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
+    r"""保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
 
     Parameters
     ----------
     datafile : str or list
         DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
     ai : int
         原子编号列表（体系中的第几号原子，不是质子数）
@@ -142,16 +140,17 @@
     dumpfile : str
         dump格式的轨迹文件名，默认为aimdTraj.dump
     icombine : bool
         是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
-    >>> from dspawpy.analysis.write import write_dump_traj
+    >>> from dspawpy.io.write import write_dump_traj
     >>> write_dump_traj(datafile='aimd.h5', ai=[1,2,3], index=1, dumpfile='aimdTraj.dump')
+    Reading E:\Dev\dspawpy\test\new\aimd.h5 ...
     """
     if isinstance(datafile, list):
         dfs = datafile
     elif isinstance(datafile, str):
         dfs = [datafile]
     else:
         raise TypeError("datafile must be a str or a list of str!")
@@ -173,20 +172,18 @@
                 print("Reading aimd.h5...")
             elif os.path.exists(os.path.join(directory, "aimd.json")):
                 df = os.path.join(directory, "aimd.json")
                 print("Reading aimd.json...")
             else:
                 raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
 
-        if df.endswith(".h5"):
-            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_h5(df, index, ele, ai)
-        elif df.endswith(".json"):
-            Nstep, eles, poses, lats, D_mag_fix = _sinfo_from_json(df, index, ele, ai)
+        if df.endswith(".h5") or df.endswith(".json"):
+            Nstep, eles, poses, lats, D_mag_fix = get_sinfo(df, index, ele, ai)
         else:
-            raise TypeError("仅支持读取h5或json文件！")
+            raise TypeError("write_dump_traj 仅支持读取h5或json文件！")
 
         # 写入文件
         with open(dumpfilename, "w") as f:
             for n in range(Nstep):
                 box_bounds = _get_lammps_non_orthogonal_box(lats[n])
                 f.write("ITEM: TIMESTEP\n%d\n" % n)
                 f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
@@ -376,15 +373,15 @@
             dataB = json.load(f3)
             rhoB = np.array(dataB["Rho"]["TotalCharge"])
     else:
         raise ValueError(f"file format must be either h5 or json: {B}")
 
     print(f"计算电荷差分...")
     rho = rhoAB - rhoA - rhoB
-    rho = np.array(rho).reshape(nGrids[0], nGrids[1], nGrids[2])
+    rho = np.array(rho).reshape(shape=(nGrids[0], nGrids[1], nGrids[2]))
 
     element = list(set(atom_symbol))
     element = sorted(set(atom_symbol), key=atom_symbol.index)
     element_num = np.zeros(len(element))
     for i in range(len(element)):
         element_num[i] = atom_symbol.count(element[i])
 
@@ -425,43 +422,89 @@
                     ind = ind + 1
                     if ind % 5 == 0:
                         out.write("\n")
 
     print(f"成功写入 {output}")
 
 
-def to_file(structure, filename: str, fmt, coords_are_cartesian=True):
-    """往结构文件中写入信息
+def to_file(structure, filename: str, fmt=None, coords_are_cartesian=True):
+    r"""往结构文件中写入信息
 
     Parameters
     ----------
     structure : Structure
         pymatgen的Structure对象
     filename : str
         结构文件名
     fmt : str
-        结构文件类型，支持 "json","as","hzw"
+        结构文件类型，目前支持 "json","as","hzw","pdb"四种类型
     coords_are_cartesian : bool
         坐标是否为笛卡尔坐标，默认为True
 
     Examples
     --------
+
+    如果不指定 fmt 参数，将尝试根据文件名后缀判断。
+
+    如果要生成 as 结构文件（可用于开始新任务），可参考如下命令:
+
+    >>> from dspawpy.io.structure import build_Structures_from_datafile
+    >>> s = build_Structures_from_datafile('neb01.h5', index=1)[0]
+    Reading E:\Dev\dspawpy\test\new\neb01.h5 ...
     >>> from dspawpy.io.write import to_file
-    >>> to_file(structure, filename='Si.json', fmt='json')
-    >>> to_file(structure, filename='Si.as', fmt='as')
-    >>> to_file(structure, filename='Si.hzw', fmt='hzw')
+    >>> to_file(s, filename='PtH.as', coords_are_cartesian=True)
+    --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.as
+
+    如果 Structure 中有磁矩或自由度信息，将会按最完整的格式统一写入，形如 Fix_x, Fix_y, Fix_z, Mag_x, Mag_y, Mag_z，自由度信息默认为 F，磁矩默认为 0.0。可视情况自行手动删除生成的 as 文件中的这些默认信息
+
+    >>> with open('PtH.as') as f:
+    ...     print(f.read())
+    ...
+    Total number of atoms
+    3
+    Lattice Fix_x Fix_y Fix_z
+    5.60580000 0.00000000 0.00000000 F F F
+    0.00000000 5.60580000 0.00000000 F F F
+    0.00000000 0.00000000 16.81740000 F F F
+    Cartesian Fix_x Fix_y Fix_z Mag
+    H 2.48770271 3.85219888 6.93647446 F F F 0.0
+    Pt 1.40145000 1.40145000 1.98192999 T T T 0.0
+    Pt 4.20434996 1.40145000 1.98192999 T T T 0.0
+
+    写成 json 文件，将忽略磁矩和自由度信息
+
+    >>> to_file(s, filename='PtH.json')
+    --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.json
+
+    写成 hzw 文件，也将忽略磁矩和自由度信息
+
+    >>> to_file(s, filename='PtH.hzw')
+    --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.hzw
+
+    写成 pdb 文件，也将忽略磁矩和自由度信息
+
+    >>> to_file(s, filename='PtH.pdb')
+    --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.pdb
     """
+
+    if fmt is None:
+        fmt = filename.split(".")[-1]
+
     if fmt == "json":
         _to_dspaw_json(structure, filename, coords_are_cartesian)
     elif fmt == "as":
         _to_dspaw_as(structure, filename, coords_are_cartesian)
     elif fmt == "hzw":
         _to_hzw(structure, filename)
     elif fmt == "pdb":
         _to_pdb(structure, filename)
+    else:
+        raise NotImplementedError(f"不支持的文件格式 {fmt}")
+
+    print(f"--> 成功写入文件 {os.path.abspath(filename)} ")
 
 
 def _write_atoms(fileobj, hdf5):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
     lattice = np.asarray(hdf5["/AtomInfo/Lattice"]).reshape(-1, 1)  # 将列表lattice下的多个列表整合
     fileobj.write(
@@ -569,50 +612,99 @@
                         break
                 file.write("\n")
 
             file.write("\n")
 
 
 def _to_dspaw_as(structure, filename: str, coords_are_cartesian=True):
-    """write dspaw as file
-    If converted from as file, will copy the mag and fix info,
-        otherwise, those info will be ignored!
-    """
+    """write dspaw structure file of .as type"""
     with open(filename, "w", encoding="utf-8") as file:
         file.write("Total number of atoms\n")
         file.write("%d\n" % len(structure))
 
-        file.write("Lattice\n")
-        for v in structure.lattice.matrix:
-            file.write("%.6f %.6f %.6f\n" % (v[0], v[1], v[2]))
+        # ^ write lattice info
+        if "LatticeFixs" in structure.sites[0].properties:
+            lfinfo = structure.sites[0].properties["LatticeFixs"]
+            if len(lfinfo) == 3:
+                file.write("Lattice Fix\n")
+                formatted_fts = []
+                for ft in lfinfo:
+                    if ft == "True":  # True
+                        ft_formatted = "T"
+                    else:
+                        ft_formatted = "F"
+                    formatted_fts.append(ft_formatted)
+                for v in structure.lattice.matrix:
+                    # write each element of formatted_fts in a line without [] symbol
+                    file.write(f'{v} {formatted_fts}.strip("[").strip("]")\n')
+            elif len(lfinfo) == 9:
+                file.write("Lattice Fix_x Fix_y Fix_z\n")
+                formatted_fts = []
+                for ft in lfinfo:
+                    if ft == "True":  # True
+                        ft_formatted = "T"
+                    else:
+                        ft_formatted = "F"
+                    formatted_fts.append(ft_formatted)
+                fix_str1 = " ".join(formatted_fts[:3])
+                fix_str2 = " ".join(formatted_fts[3:6])
+                fix_str3 = " ".join(formatted_fts[6:9])
+                v1 = structure.lattice.matrix[0]
+                v2 = structure.lattice.matrix[1]
+                v3 = structure.lattice.matrix[2]
+                file.write(f" {v1[0]:5.8f} {v1[1]:5.8f} {v1[2]:5.8f} {fix_str1}\n")
+                file.write(f" {v2[0]:5.8f} {v2[1]:5.8f} {v2[2]:5.8f} {fix_str2}\n")
+                file.write(f" {v3[0]:5.8f} {v3[1]:5.8f} {v3[2]:5.8f} {fix_str3}\n")
+            else:
+                raise ValueError(
+                    f"LatticeFixs should be a list of 3 or 9 bools, but got {lfinfo}"
+                )
+        else:
+            file.write("Lattice\n")
+            for v in structure.lattice.matrix:
+                file.write("%.8f %.8f %.8f\n" % (v[0], v[1], v[2]))
 
         i = 0
         for site in structure:
+            keys = []
+            for key in site.properties:  # site.properties is a dictionary
+                if key != "LatticeFixs":
+                    keys.append(key)
+            keys.sort()
+            keys_str = " ".join(keys)  # sth like 'magmom fix
             if i == 0:
-                if "line6s" in site.properties:
-                    file.write("%s\n" % site.properties["line6s"])
+                if coords_are_cartesian:
+                    file.write(f"Cartesian {keys_str}\n")
                 else:
-                    if coords_are_cartesian:
-                        file.write("Cartesian\n")
-                    else:
-                        file.write("Direct\n")
+                    file.write(f"Direct {keys_str}\n")
             i += 1
 
             coords = site.coords if coords_are_cartesian else site.frac_coords
-            if "others" in site.properties:
-                sp = " ".join(site.properties["others"])  # flatten str list
-                file.write(
-                    "%s %.6f %.6f %.6f %s\n"
-                    % (site.species_string, coords[0], coords[1], coords[2], sp)
-                )
-            else:  # the most common case
-                file.write(
-                    "%s %.6f %.6f %.6f\n"
-                    % (site.species_string, coords[0], coords[1], coords[2])
-                )
+            raw = []
+            for sortted_key in keys:  # site.properties is a dictionary
+                raw_values = site.properties[sortted_key]
+                # print(f'{raw_values=}')
+                if isinstance(raw_values, list):  # single True or False
+                    values = raw_values
+                else:
+                    values = [raw_values]
+                for v in values:
+                    if v == "True":
+                        value_str = "T"
+                    elif v == "False":
+                        value_str = "F"
+                    else:
+                        value_str = str(v)
+                    raw.append(value_str)
+
+            final_strs = " ".join(raw)  # sth like '0.0 T
+            file.write(
+                "%s %.8f %.8f %.8f %s\n"
+                % (site.species_string, coords[0], coords[1], coords[2], final_strs)
+            )
 
 
 def _to_hzw(structure, filename: str):
     with open(filename, "w", encoding="utf-8") as file:
         file.write("% The number of probes \n")
         file.write("0\n")
         file.write("% Uni-cell vector\n")
@@ -642,14 +734,16 @@
     d = {"Lattice": lattice, "CoordinateType": coordinate_type, "Atoms": atoms}
 
     with open(filename, "w", encoding="utf-8") as file:
         json.dump(d, file, indent=4)
 
 
 def _to_pdb(structures, pdb_filename: str):
+    if not isinstance(structures, list):
+        structures = [structures]
     with open(pdb_filename, "w", encoding="utf-8") as file:
         for i, s in enumerate(structures):
             file.write("MODEL         %d\n" % (i + 1))
             file.write("REMARK   Converted from Structures\n")
             file.write("REMARK   Converted using dspawpy\n")
             lengths = s.lattice.lengths
             angles = s.lattice.angles
```

## Comparing `dspawpy-0.9.1.dist-info/METADATA` & `dspawpy-0.9.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
@@ -27,14 +27,19 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 0.9.2
+
+- 新增功能： 支持从as文件中解析磁矩和FIX信息
+- 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
+
 ### 0.9.1
 
 - 重要变更： 精简合并多个函数，统一调用方法
 - 新增功能： 支持合并多个xyz和dump文件
 - 细节优化： 读取h5或json文件后若无错误，不再打印空行
 - 细节优化： 耗时的RDF计算显示进度百分比
```

## Comparing `dspawpy-0.9.1.dist-info/RECORD` & `dspawpy-0.9.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 dspawpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/plot.py,sha256=ocLkU08WfMb2fyETrBSSZvxZFSg2sPX8rLusXZLT5BM,29208
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/analysis/aimdtools.py,sha256=vNSr_6lKBGEsfmxzN2EjQQCEhtwxflxNseJCPTiU614,24557
+dspawpy/analysis/aimdtools.py,sha256=9AMUG7Eeesgyj86MDtWDZ9EpsOkJ86cMNFwqpeMUr-M,24571
 dspawpy/analysis/vacf.py,sha256=g5IS6Q7QGYa17XBVnYEH-MubGSpkUsDPpMaI_ELacw4,20152
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/diffusion/neb.py,sha256=U6J7lSlE_xp1rCON5mgfWWi5DFHVZYVb5xjqLlGxXXI,3592
 dspawpy/diffusion/nebtools.py,sha256=tfQCQPUmZKELz7ImwyiJiiFfXahC9U3doarExspL-DU,53467
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/io/read.py,sha256=BfyiGH-aJLjQAMMNAF9tuThQHIyJGzCa6R0zzqkXMpE,48925
+dspawpy/io/read.py,sha256=uVkODhh8IPU8k4Np31a-FFYF8SNK7wOe-gDOV49D-DU,52393
 dspawpy/io/read_json.py,sha256=2bcNQP51SR2yMyFE7c2TIutYp93K8IH-dpLmH5yy4bo,7721
-dspawpy/io/structure.py,sha256=HqhBLKqAJcHclFCZH4lEiaX7yR_qv8ygACOsPHyLKn0,6163
+dspawpy/io/structure.py,sha256=vm_GKQqFvvGRjUQx3_pSn9eI2eEc8ZiX-z-71lbHF5s,8538
 dspawpy/io/utils.py,sha256=FdbFbZqKfnDOGBJ4OaKD-4IBAAlqjtQ0l1NppvkMKOM,25241
-dspawpy/io/write.py,sha256=CKgyqSGFvjkIcrzeeVDyZS4W2Otvpz1FlewlPOqieP0,24416
+dspawpy/io/write.py,sha256=W70yWfHDhQ2n8YItr80ubPhV591ClbvcmfKBAnapND8,28491
 dspawpy/io/write_json.py,sha256=n3GhdDnFFtW7eY4U5u7czdlpbSWnsGP7WUD5eS1ZmqI,1761
-dspawpy-0.9.1.dist-info/METADATA,sha256=EQov-UB9e9O0p886lOUr6Oj9MDfA-PJyMgfyTlVSVIk,2036
-dspawpy-0.9.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-0.9.1.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-0.9.1.dist-info/RECORD,,
+dspawpy-0.9.2.dist-info/METADATA,sha256=Ad4kzjShQczca8QTJtZCHROpU6VkZwUZVFjIkI4Z1Wk,2215
+dspawpy-0.9.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-0.9.2.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-0.9.2.dist-info/RECORD,,
```

