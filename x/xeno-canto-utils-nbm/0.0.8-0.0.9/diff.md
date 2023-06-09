# Comparing `tmp/xeno_canto_utils_nbm-0.0.8.tar.gz` & `tmp/xeno_canto_utils_nbm-0.0.9.tar.gz`

## Comparing `xeno_canto_utils_nbm-0.0.8.tar` & `xeno_canto_utils_nbm-0.0.9.tar`

### file list

```diff
@@ -1,241 +1,241 @@
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/.remi/.gitignore
--rwxr-xr-x   0        0        0     5999 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/.remi/config.yaml
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/.remi/exclude.txt
--rwxr-xr-x   0        0        0     6171 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/.remi/last_push.log
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/__init__.py
--rwxr-xr-x   0        0        0     8934 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/ia_model_utils.py
--rwxr-xr-x   0        0        0     9437 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/train.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/__init__.py
--rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/faster_rcnn.py
--rwxr-xr-x   0        0        0    11382 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/faster_utils.py
--rwxr-xr-x   0        0        0    32813 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/layers.py
--rwxr-xr-x   0        0        0    14631 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/resnet_backbone.py
--rwxr-xr-x   0        0        0     9151 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/vgg_backbone.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/__init__.py
--rwxr-xr-x   0        0        0     9075 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/image_dataset.py
--rwxr-xr-x   0        0        0    19491 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/prepare_dataset.py
--rwxr-xr-x   0        0        0    12603 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/utils.py
--rwxr-xr-x   0        0        0     9081 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/xeno_canto_utils.py
--rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/file_ids.json
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/file_ids_bruits.json
--rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/anthus_hodgsoni_E/anthus_hodgsoni#759611.txt
--rwxr-xr-x   0        0        0      198 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_A/carduelis_carduelis#610337.txt
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#495511.txt
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#631728.txt
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#643389.txt
--rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#736650.txt
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#767094.txt
--rwxr-xr-x   0        0        0     1125 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#784874.txt
--rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#508267.txt
--rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#593783.txt
--rwxr-xr-x   0        0        0      464 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#627460.txt
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_D/carduelis_carduelis#553808.txt
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_D/carduelis_carduelis#589186.txt
--rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#526268.txt
--rwxr-xr-x   0        0        0      473 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#576514.txt
--rwxr-xr-x   0        0        0     1707 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#639993.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#642402.txt
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#643242.txt
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#646637.txt
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#667960.txt
--rwxr-xr-x   0        0        0      133 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#667962.txt
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#670479.txt
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#670659.txt
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#671224.txt
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#673160.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#674601.txt
--rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687106.txt
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687108.txt
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687112.txt
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687118.txt
--rwxr-xr-x   0        0        0   198224 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#693070.mp3
--rwxr-xr-x   0        0        0      339 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#722002.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#722841.txt
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#723925.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#724516.txt
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#725953.txt
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#737090.txt
--rwxr-xr-x   0        0        0     1302 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#740387.txt
--rwxr-xr-x   0        0        0   226511 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#748313.mp3
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#754947.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757044.txt
--rwxr-xr-x   0        0        0      539 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757873.txt
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#759884.txt
--rwxr-xr-x   0        0        0      603 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#439319.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#443980.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#533607.txt
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#553226.txt
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#555747.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#556883.txt
--rwxr-xr-x   0        0        0     2721 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#563722.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585127.txt
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585960.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#647150.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#649364.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#673846.txt
--rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#702752.txt
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#747803.txt
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#750838.txt
--rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#465609.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#553346.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#585145.txt
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#585281.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#593886.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#744668.txt
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#443244.txt
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#539208.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#585986.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#587358.txt
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#598360.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#612711.txt
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#626192.txt
--rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#628004.txt
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#685857.txt
--rwxr-xr-x   0        0        0    16534 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#705756.txt
--rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#707779.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#709772.txt
--rwxr-xr-x   0        0        0      448 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#747094.txt
--rwxr-xr-x   0        0        0     3620 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#772153.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#781870.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#444457.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#542163.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#589087.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#593281.txt
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#616231.txt
--rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#626193.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#681055.txt
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#691390.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#780673.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#673472.txt
--rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#681529.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#700848.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_E/fringilla_coelebs#679432.txt
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#505628.txt
--rwxr-xr-x   0        0        0     2704 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#543940.txt
--rwxr-xr-x   0        0        0   138672 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.mp3
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.txt
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#632885.txt
--rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#668899.txt
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_C/linaria_cannabina#756792.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_D/linaria_cannabina#679344.txt
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_D/linaria_cannabina#760424.txt
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_E/linaria_cannabina#595795.txt
--rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#246977.txt
--rwxr-xr-x   0        0        0      831 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#510684.txt
--rwxr-xr-x   0        0        0     2217 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#606298.txt
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#492310.txt
--rwxr-xr-x   0        0        0      473 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#503591.txt
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#538439.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#541525.txt
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#549027.txt
--rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552837.txt
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552841.txt
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#583387.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#583963.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#586086.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#588185.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#594114.txt
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#595052.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#603557.txt
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#604642.txt
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#623717.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#625964.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#644273.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#649542.txt
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#667181.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#667182.txt
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673408.txt
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673409.txt
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673412.txt
--rwxr-xr-x   0        0        0      677 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673414.txt
--rwxr-xr-x   0        0        0      410 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673416.txt
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673417.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673436.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#678221.txt
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#702765.txt
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#741190.txt
--rwxr-xr-x   0        0        0      404 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#742562.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#742565.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#743946.txt
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#745393.txt
--rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#748708.txt
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#749914.txt
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#761705.txt
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#785288.txt
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#493546.txt
--rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#549790.txt
--rwxr-xr-x   0        0        0      536 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#555762.txt
--rwxr-xr-x   0        0        0      406 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#580611.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#583890.txt
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#617925.txt
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#755488.txt
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_E/pluvialis_squatarola#604694.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#436944.txt
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#488271.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#645041.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#645436.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#668818.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#704169.txt
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#708608.txt
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#708968.txt
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#710803.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#710815.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#730640.txt
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#782190.txt
--rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#784107.txt
--rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#785589.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#786602.txt
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787130.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787167.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787323.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787672.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787711.txt
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#789124.txt
--rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#790674.txt
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#791079.txt
--rwxr-xr-x   0        0        0      310 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#791540.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#792778.txt
--rwxr-xr-x   0        0        0     1008 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#793494.txt
--rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#794338.txt
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#794945.txt
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#795134.txt
--rwxr-xr-x   0        0        0     1819 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/tringa_totanus_E/tringa_totanus#544307.txt
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/tringa_totanus_E/tringa_totanus#544614.txt
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#436941.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#505625.txt
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#506434.txt
--rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#507660.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#534139.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#540169.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#541231.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#542005.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#543243.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#544791.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#547913.txt
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#549196.txt
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#591995.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#594848.txt
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#596142.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#622550.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#638857.txt
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#644653.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#672774.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#676570.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#681860.txt
--rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#714652.txt
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#721330.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#723223.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#754337.txt
--rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_D/turdus_torquatus#757161.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#435844.txt
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#500815.txt
--rwxr-xr-x   0        0        0      310 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#542731.txt
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#550010.txt
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#595699.txt
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/new_XC_ds/turdus_torquatus_E/turdus_torquatus#629701.txt
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/xeno_canto_utils_nbm/__init__.py
--rwxr-xr-x   0        0        0     4405 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/xeno_canto_utils_nbm/xeno_canto_utils.py
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/LICENSE
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/README.md
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/.remi/.gitignore
+-rwxr-xr-x   0        0        0     5999 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/.remi/config.yaml
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/.remi/exclude.txt
+-rwxr-xr-x   0        0        0     6171 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/.remi/last_push.log
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/__init__.py
+-rwxr-xr-x   0        0        0     8934 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/ia_model_utils.py
+-rwxr-xr-x   0        0        0     9437 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/train.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/__init__.py
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/faster_rcnn.py
+-rwxr-xr-x   0        0        0    11382 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/faster_utils.py
+-rwxr-xr-x   0        0        0    32813 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/layers.py
+-rwxr-xr-x   0        0        0    14631 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/resnet_backbone.py
+-rwxr-xr-x   0        0        0     9151 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/vgg_backbone.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/__init__.py
+-rwxr-xr-x   0        0        0     9075 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/image_dataset.py
+-rwxr-xr-x   0        0        0    19491 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/prepare_dataset.py
+-rwxr-xr-x   0        0        0    12603 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/utils.py
+-rwxr-xr-x   0        0        0     9081 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/xeno_canto_utils.py
+-rwxr-xr-x   0        0        0     2210 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/file_ids.json
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/file_ids_bruits.json
+-rwxr-xr-x   0        0        0      391 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/anthus_hodgsoni_E/anthus_hodgsoni#759611.txt
+-rwxr-xr-x   0        0        0      198 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_A/carduelis_carduelis#610337.txt
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#495511.txt
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#631728.txt
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#643389.txt
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#736650.txt
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#767094.txt
+-rwxr-xr-x   0        0        0     1125 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#784874.txt
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#508267.txt
+-rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#593783.txt
+-rwxr-xr-x   0        0        0      464 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#627460.txt
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_D/carduelis_carduelis#553808.txt
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_D/carduelis_carduelis#589186.txt
+-rwxr-xr-x   0        0        0       68 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#526268.txt
+-rwxr-xr-x   0        0        0      473 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#576514.txt
+-rwxr-xr-x   0        0        0     1707 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#639993.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#642402.txt
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#643242.txt
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#646637.txt
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#667960.txt
+-rwxr-xr-x   0        0        0      133 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#667962.txt
+-rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#670479.txt
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#670659.txt
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#671224.txt
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#673160.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#674601.txt
+-rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687106.txt
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687108.txt
+-rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687112.txt
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687118.txt
+-rwxr-xr-x   0        0        0   198224 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#693070.mp3
+-rwxr-xr-x   0        0        0      339 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#722002.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#722841.txt
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#723925.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#724516.txt
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#725953.txt
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#737090.txt
+-rwxr-xr-x   0        0        0     1302 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#740387.txt
+-rwxr-xr-x   0        0        0   226511 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#748313.mp3
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#754947.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757044.txt
+-rwxr-xr-x   0        0        0      539 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757873.txt
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#759884.txt
+-rwxr-xr-x   0        0        0      603 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#439319.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#443980.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#533607.txt
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#553226.txt
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#555747.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#556883.txt
+-rwxr-xr-x   0        0        0     2721 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#563722.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585127.txt
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585960.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#647150.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#649364.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#673846.txt
+-rwxr-xr-x   0        0        0      749 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#702752.txt
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#747803.txt
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#750838.txt
+-rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#465609.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#553346.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#585145.txt
+-rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#585281.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#593886.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#744668.txt
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#443244.txt
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#539208.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#585986.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#587358.txt
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#598360.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#612711.txt
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#626192.txt
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#628004.txt
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#685857.txt
+-rwxr-xr-x   0        0        0    16534 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#705756.txt
+-rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#707779.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#709772.txt
+-rwxr-xr-x   0        0        0      448 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#747094.txt
+-rwxr-xr-x   0        0        0     3620 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#772153.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#781870.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#444457.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#542163.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#589087.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#593281.txt
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#616231.txt
+-rwxr-xr-x   0        0        0      326 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#626193.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#681055.txt
+-rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#691390.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#780673.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#673472.txt
+-rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#681529.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_D/fringilla_coelebs#700848.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_E/fringilla_coelebs#679432.txt
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#505628.txt
+-rwxr-xr-x   0        0        0     2704 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#543940.txt
+-rwxr-xr-x   0        0        0   138672 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.mp3
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.txt
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#632885.txt
+-rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#668899.txt
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_C/linaria_cannabina#756792.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_D/linaria_cannabina#679344.txt
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_D/linaria_cannabina#760424.txt
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_E/linaria_cannabina#595795.txt
+-rwxr-xr-x   0        0        0      704 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#246977.txt
+-rwxr-xr-x   0        0        0      831 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#510684.txt
+-rwxr-xr-x   0        0        0     2217 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#606298.txt
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#492310.txt
+-rwxr-xr-x   0        0        0      473 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#503591.txt
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#538439.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#541525.txt
+-rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#549027.txt
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552837.txt
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552841.txt
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#583387.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#583963.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#586086.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#588185.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#594114.txt
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#595052.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#603557.txt
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#604642.txt
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#623717.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#625964.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#644273.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#649542.txt
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#667181.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#667182.txt
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673408.txt
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673409.txt
+-rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673412.txt
+-rwxr-xr-x   0        0        0      677 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673414.txt
+-rwxr-xr-x   0        0        0      410 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673416.txt
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673417.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673436.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#678221.txt
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#702765.txt
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#741190.txt
+-rwxr-xr-x   0        0        0      404 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#742562.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#742565.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#743946.txt
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#745393.txt
+-rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#748708.txt
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#749914.txt
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#761705.txt
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#785288.txt
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#493546.txt
+-rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#549790.txt
+-rwxr-xr-x   0        0        0      536 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#555762.txt
+-rwxr-xr-x   0        0        0      406 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#580611.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#583890.txt
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#617925.txt
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#755488.txt
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_E/pluvialis_squatarola#604694.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#436944.txt
+-rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#488271.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#645041.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#645436.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#668818.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#704169.txt
+-rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#708608.txt
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#708968.txt
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#710803.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#710815.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#730640.txt
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#782190.txt
+-rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#784107.txt
+-rwxr-xr-x   0        0        0     1021 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#785589.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#786602.txt
+-rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787130.txt
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787167.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787323.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787672.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#787711.txt
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#789124.txt
+-rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#790674.txt
+-rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#791079.txt
+-rwxr-xr-x   0        0        0      310 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#791540.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#792778.txt
+-rwxr-xr-x   0        0        0     1008 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#793494.txt
+-rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#794338.txt
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#794945.txt
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#795134.txt
+-rwxr-xr-x   0        0        0     1819 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/tringa_totanus_E/tringa_totanus#544307.txt
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/tringa_totanus_E/tringa_totanus#544614.txt
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#436941.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#505625.txt
+-rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#506434.txt
+-rwxr-xr-x   0        0        0      315 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#507660.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#534139.txt
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#540169.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#541231.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#542005.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#543243.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#544791.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#547913.txt
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#549196.txt
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#591995.txt
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#594848.txt
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#596142.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#622550.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#638857.txt
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#644653.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#672774.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#676570.txt
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#681860.txt
+-rwxr-xr-x   0        0        0      127 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#714652.txt
+-rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#721330.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#723223.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#754337.txt
+-rwxr-xr-x   0        0        0      128 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_D/turdus_torquatus#757161.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#435844.txt
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#500815.txt
+-rwxr-xr-x   0        0        0      310 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#542731.txt
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#550010.txt
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#595699.txt
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/new_XC_ds/turdus_torquatus_E/turdus_torquatus#629701.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/xeno_canto_utils_nbm/__init__.py
+-rwxr-xr-x   0        0        0     4405 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/xeno_canto_utils_nbm/xeno_canto_utils.py
+-rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/LICENSE
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/README.md
+-rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 xeno_canto_utils_nbm-0.0.9/PKG-INFO
```

### Comparing `xeno_canto_utils_nbm-0.0.8/.remi/config.yaml` & `xeno_canto_utils_nbm-0.0.9/.remi/config.yaml`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/.remi/last_push.log` & `xeno_canto_utils_nbm-0.0.9/.remi/last_push.log`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/ia_model_utils.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/ia_model_utils.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/train.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/train.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/faster_rcnn.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/faster_utils.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/faster_utils.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/layers.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/layers.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/resnet_backbone.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/resnet_backbone.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/nets/vgg_backbone.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/nets/vgg_backbone.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/image_dataset.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/prepare_dataset.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/prepare_dataset.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/utils.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/nbm_ia_v2/pytorch_dataset/xeno_canto_utils.py` & `xeno_canto_utils_nbm-0.0.9/nbm_ia_v2/pytorch_dataset/xeno_canto_utils.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/file_ids.json` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/file_ids.json`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#784874.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_B/carduelis_carduelis#784874.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#593783.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/carduelis_carduelis_C/carduelis_carduelis#593783.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#639993.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#639993.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#646637.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#646637.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687106.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687106.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687112.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#687112.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#693070.mp3` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#693070.mp3`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#740387.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#740387.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#748313.mp3` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#748313.mp3`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#754947.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#754947.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757873.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_A/charadrius_hiaticula#757873.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#439319.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#439319.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#555747.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#555747.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#563722.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#563722.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585960.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#585960.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#702752.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_D/charadrius_hiaticula#702752.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#465609.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/charadrius_hiaticula_E/charadrius_hiaticula#465609.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#539208.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#539208.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#628004.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#628004.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#705756.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#705756.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#707779.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#707779.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#772153.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_B/fringilla_coelebs#772153.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#616231.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#616231.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#691390.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/fringilla_coelebs_C/fringilla_coelebs#691390.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#543940.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#543940.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.mp3` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#583333.mp3`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#632885.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#632885.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_B/linaria_cannabina#668899.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_B/linaria_cannabina#668899.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_D/linaria_cannabina#760424.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_D/linaria_cannabina#760424.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_E/linaria_cannabina#595795.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_E/linaria_cannabina#595795.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#246977.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#246977.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#510684.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#510684.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#606298.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/linaria_cannabina_cf_A/linaria_cannabina#606298.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#492310.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#492310.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552837.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#552837.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673408.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673408.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673414.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673414.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673417.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#673417.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#741190.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#741190.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#748708.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_C/pluvialis_squatarola#748708.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#549790.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#549790.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#555762.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/pluvialis_squatarola_D/pluvialis_squatarola#555762.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#785589.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#785589.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#790674.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#790674.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#793494.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/rallus_aquaticus_A/rallus_aquaticus#793494.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/new_XC_ds/tringa_totanus_E/tringa_totanus#544307.txt` & `xeno_canto_utils_nbm-0.0.9/new_XC_ds/tringa_totanus_E/tringa_totanus#544307.txt`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/xeno_canto_utils_nbm/xeno_canto_utils.py` & `xeno_canto_utils_nbm-0.0.9/xeno_canto_utils_nbm/xeno_canto_utils.py`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/LICENSE` & `xeno_canto_utils_nbm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno_canto_utils_nbm-0.0.8/pyproject.toml` & `xeno_canto_utils_nbm-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,27 @@
     ]
 build-backend = "hatchling.build"
 
 [project]
 name = "xeno_canto_utils_nbm"
 description = "Utility functions to interact with the Xeno Canto API with python"
 
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "Louloulou", email = "laerien@gmail.com" }
 ]
 readme = "README.md"
 license = { text = "GNU General Public License v3.0" }
 keywords = [ "machine learning for biology" ]
 
 dependencies = [
     "numpy",
-    "requests"
+    "requests",
+    "ffmpeg",
+    "ffmpeg-python"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/LouisBearing/BirdSoundClassif"
 
 [project.scripts]
 xeno = "xeno_canto_utils_nbm.xeno_canto_utils:main"
```

### Comparing `xeno_canto_utils_nbm-0.0.8/PKG-INFO` & `xeno_canto_utils_nbm-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: xeno_canto_utils_nbm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utility functions to interact with the Xeno Canto API with python
 Project-URL: Homepage, https://github.com/LouisBearing/BirdSoundClassif
 Author-email: Louloulou <laerien@gmail.com>
 License: GNU General Public License v3.0
 License-File: LICENSE
 Keywords: machine learning for biology
+Requires-Dist: ffmpeg
+Requires-Dist: ffmpeg-python
 Requires-Dist: numpy
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # BirdSoundClassif
 
 How to install the package:
```

