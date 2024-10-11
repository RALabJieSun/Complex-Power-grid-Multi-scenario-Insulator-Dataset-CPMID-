# Complex-Power-grid-Multi-scenario-Insulator-Dataset(CPMID)

# 1. **DATASET OVERVIEW**

​	The Complex Power-grid Multi-scenario Insulator Dataset(CPMID) consists of labeled high-quality images of Complex Power-grid Multi-scenario Insulators. These images primarily involve insulator strings and two types of defects. The labels in the CPMID dataset contain three categories:

1. Insulator strings
2. Broken defects
3. Flashover damages

​	This readme document provides the dataset overview, characteristics, file structure and labeling format for CPMID, not the imagery itself.

# 2. **DATASET DETAILS**

​	To enhance the model's performance in detecting insulators and their defects in complex, multi-scenario power grid environments during actual deployment, it is essential to develop a more generalized and higher-quality insulator dataset. Previous researchers have limited the definition of insulators in complex scenes to small targets and background interferenc. However, the characteristics of insulators in such environments also include dense distribution, overlapping, occlusion, and large-scale variations. Additionally, exiting publicly available insulator datasets, such as the IDID and CPLID datasets, primarily focus on insulators in overhead transmission lines. Nonetheless, insulators are critical components in transmission networks and distribution networks, substation plants, and power plants. To address these limitations, we have developed the Complex Power-grid Multi-scenario Insulator Dataset (CPMID), as depicted in Fig 2-1. This benchmark dataset encompasses a broader range of insulator types and a more diverse array of scenarios. 

​	The insulator and defect dataset, developed for complex, multi-scenario power grid environments, was utilized to pre-train existing insulator detection models. Analysis revealed a significant imbalance in the number of labels for normal insulators compared to those for damaged and pollution flashover defects. This imbalance led to issues such as non-converging accuracy curves, low recall rates, and overfitting on the validation set during model training. To address this issue, this dataset incorporates defect samples from public insulator datasets into the individual dataset to increase the label count for damaged and pollution flashover defects. This strategy aims to mitigate the effects of label imbalance and enhance the model's ability to learn and detect features of both defect types. Table 2-1 lists the objectives, power grid scenarios, number of images, etc. of the CPMID compared to the other publicly available dataset. The data indicate that the integrated insulator dataset is more suitable for ongoing research in complex power grid scenarios than the dataset before integration.

<img src='Fig/L_Self-constructed insulator datasets for complex, multi-scenario power grid environments.png'>

<div align=center><strong>Fig.</strong> Sample visualization in CPMID  for complex, multi-scenario power grid environments.</div>

<br>

<div align=center><strong>Table</strong> Statistics details of CPMID compared with other publicly available insulator datasets.</div>

<table>
  <tr>
    <th>Characteristic</th>
    <th>CPLID (public)</th>
    <th>IDID (public)</th>
    <th>CPMID (ours)</th>
  </tr>
  <tr>
    <td><strong>Power grid scenario</strong></td>
    <td>Transmission networks</td>
    <td>Transmission networks, Distribution networks</td>
    <td>Transmission networks, Distribution networks, Substation plants, Power plants</td>
  </tr>
  <tr>
    <td><strong>Feature</strong></td>
    <td>Sample imbalance</td>
    <td>Small targets, dense, background interference</td>
    <td>Dense, overlapped, sheltered, cross-scale, background interference, small targets, sample imbalance</td>
  </tr>
  <tr>
    <td><strong>Insulator strings</strong></td>
    <td>1368</td>
    <td>1891</td>
    <td>72596</td>
  </tr>
  <tr>
    <td><strong>Broken defect</strong></td>
    <td>248</td>
    <td>1204</td>
    <td>2104</td>
  </tr>
  <tr>
    <td><strong>Flashover damage</strong></td>
    <td>&mdash;</td>
    <td>2093</td>
    <td>2596</td>
  </tr>
  <tr>
    <td><strong>Total objects</strong></td>
    <td>1616</td>
    <td>8001</td>
    <td>77296</td>
  </tr>
  <tr>
    <td><strong>Total images</strong></td>
    <td>848</td>
    <td>1684</td>
    <td>7712</td>
  </tr>
  <tr>
    <td><strong>Difficulty of detection</strong></td>
    <td>Low difficulty</td>
    <td>Medium difficulty</td>
    <td>High difficulty</td>
  </tr>
</table>


# 3. **FILE STRUCTURE**

​	The dataset contains 2 folders named Annotations and Images. Table 3-1 describes the contents of the two folders.

<div align=center>Table 3-1 Composition of the dataset folder</div>

|   Folder    |                       Contents                       |
| :---------: | :--------------------------------------------------: |
| Annotations | The folder contains the labels used for the dataset  |
|   Images    | The folder contains the images used for the dataset. |

# 4. Copyright Statement

The dataset is utilized exclusively for scientific research purposes. If used, proper citation in the literature is required. Please cite it as follows: **论文引用格式**

# 5. DOWNLOAD

File shared via Netflix:  CPMID.rar.
Link: https://pan.baidu.com/s/1BABa6yUe_PwI7HhiMMdHsA Extract code: 9wpp