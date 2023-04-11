# Comparing `tmp/deep_training-0.1.1-py3-none-any.whl.zip` & `tmp/deep_training-0.1.2rc0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,138 +1,146 @@
-Zip file size: 223846 bytes, number of entries: 136
--rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-22 10:40 deep_training/__init__.py
--rw-rw-rw-  2.0 fat      874 b- defN 23-Apr-07 11:24 deep_training/setup.py
--rw-rw-rw-  2.0 fat       55 b- defN 23-Mar-19 08:44 deep_training/cv/__init__.py
--rw-rw-rw-  2.0 fat      195 b- defN 23-Mar-19 08:44 deep_training/data_helper/__init__.py
--rw-rw-rw-  2.0 fat    29088 b- defN 23-Apr-02 08:38 deep_training/data_helper/data_helper.py
--rw-rw-rw-  2.0 fat     4926 b- defN 23-Mar-19 08:44 deep_training/data_helper/data_module.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Mar-19 08:44 deep_training/data_helper/data_writer.py
--rw-rw-rw-  2.0 fat    12513 b- defN 23-Mar-24 16:06 deep_training/data_helper/training_args.py
--rw-rw-rw-  2.0 fat       70 b- defN 23-Mar-19 08:44 deep_training/nlp/__init__.py
--rw-rw-rw-  2.0 fat       56 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/__init__.py
--rw-rw-rw-  2.0 fat      241 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/activate.py
--rw-rw-rw-  2.0 fat    13271 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/crf.py
--rw-rw-rw-  2.0 fat     4653 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/handshakingkernel.py
--rw-rw-rw-  2.0 fat      435 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/mask.py
--rw-rw-rw-  2.0 fat     1319 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/mhslayer.py
--rw-rw-rw-  2.0 fat     5911 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/norm.py
--rw-rw-rw-  2.0 fat     1220 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/prefix_encoder.py
--rw-rw-rw-  2.0 fat     7259 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/seq_pointer.py
--rw-rw-rw-  2.0 fat     3550 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/w2ner.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-07 10:47 deep_training/nlp/layers/adalora/__init__.py
--rw-rw-rw-  2.0 fat    15143 b- defN 23-Apr-07 10:47 deep_training/nlp/layers/adalora/layers.py
--rw-rw-rw-  2.0 fat       72 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/lora/__init__.py
--rw-rw-rw-  2.0 fat    15095 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/lora/layers.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Mar-19 08:44 deep_training/nlp/layers/lora/utils.py
--rw-rw-rw-  2.0 fat     3662 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/BatchAllTripletLoss.py
--rw-rw-rw-  2.0 fat     3880 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
--rw-rw-rw-  2.0 fat     8358 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/BatchHardTripletLoss.py
--rw-rw-rw-  2.0 fat     4552 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/BatchSemiHardTripletLoss.py
--rw-rw-rw-  2.0 fat     2255 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/ContrastiveLoss.py
--rw-rw-rw-  2.0 fat     4573 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/ContrastiveTensionLoss.py
--rw-rw-rw-  2.0 fat     1359 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/CosineSimilarityLoss.py
--rw-rw-rw-  2.0 fat      742 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/MSELoss.py
--rw-rw-rw-  2.0 fat     1315 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/MarginMSELoss.py
--rw-rw-rw-  2.0 fat     5302 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/MegaBatchMarginLoss.py
--rw-rw-rw-  2.0 fat     2420 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/MultipleNegativesRankingLoss.py
--rw-rw-rw-  2.0 fat     2905 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/MultipleNegativesSymmetricRankingLoss.py
--rw-rw-rw-  2.0 fat     1863 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/OnlineContrastiveLoss.py
--rw-rw-rw-  2.0 fat     2880 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/SoftmaxLoss.py
--rw-rw-rw-  2.0 fat     2306 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/TripletLoss.py
--rw-rw-rw-  2.0 fat      599 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/__init__.py
--rw-rw-rw-  2.0 fat      661 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/bce_loss.py
--rw-rw-rw-  2.0 fat     1397 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/center_loss.py
--rw-rw-rw-  2.0 fat     1772 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/circle_loss.py
--rw-rw-rw-  2.0 fat     1056 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/contrast.py
--rw-rw-rw-  2.0 fat      619 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/dice_loss.py
--rw-rw-rw-  2.0 fat      710 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/focal_loss.py
--rw-rw-rw-  2.0 fat      882 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/label_smoothing.py
--rw-rw-rw-  2.0 fat      547 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/lm_loss.py
--rw-rw-rw-  2.0 fat     2149 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_arcface.py
--rw-rw-rw-  2.0 fat      962 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_casrel.py
--rw-rw-rw-  2.0 fat     1496 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_cosent.py
--rw-rw-rw-  2.0 fat     1912 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_cosface.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_globalpointer.py
--rw-rw-rw-  2.0 fat     6020 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_infonce.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_kl.py
--rw-rw-rw-  2.0 fat     1270 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_mhslinker.py
--rw-rw-rw-  2.0 fat      617 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_r-drop.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_sphereface.py
--rw-rw-rw-  2.0 fat      562 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_splinker.py
--rw-rw-rw-  2.0 fat    10822 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_spn4re.py
--rw-rw-rw-  2.0 fat     5644 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/loss_tplinker.py
--rw-rw-rw-  2.0 fat     2466 b- defN 23-Mar-19 08:44 deep_training/nlp/losses/utils.py
--rw-rw-rw-  2.0 fat       71 b- defN 23-Mar-19 08:44 deep_training/nlp/metrics/__init__.py
--rw-rw-rw-  2.0 fat      655 b- defN 23-Mar-19 08:44 deep_training/nlp/metrics/pointer.py
--rw-rw-rw-  2.0 fat       58 b- defN 23-Mar-19 08:44 deep_training/nlp/models/__init__.py
--rw-rw-rw-  2.0 fat     6811 b- defN 23-Mar-19 08:44 deep_training/nlp/models/casrel.py
--rw-rw-rw-  2.0 fat     5078 b- defN 23-Mar-19 08:44 deep_training/nlp/models/crf_cascad.py
--rw-rw-rw-  2.0 fat     1573 b- defN 23-Mar-19 08:44 deep_training/nlp/models/crf_model.py
--rw-rw-rw-  2.0 fat    12970 b- defN 23-Mar-19 08:44 deep_training/nlp/models/diffcse.py
--rw-rw-rw-  2.0 fat     5388 b- defN 23-Mar-29 16:13 deep_training/nlp/models/esimcse.py
--rw-rw-rw-  2.0 fat     4194 b- defN 23-Mar-19 08:44 deep_training/nlp/models/gec_model.py
--rw-rw-rw-  2.0 fat    10824 b- defN 23-Mar-19 08:44 deep_training/nlp/models/gplinker.py
--rw-rw-rw-  2.0 fat     3799 b- defN 23-Mar-19 08:44 deep_training/nlp/models/infonce.py
--rw-rw-rw-  2.0 fat     2444 b- defN 23-Mar-19 08:44 deep_training/nlp/models/mhs_ner.py
--rw-rw-rw-  2.0 fat     5976 b- defN 23-Mar-19 08:44 deep_training/nlp/models/mhslinker.py
--rw-rw-rw-  2.0 fat     4646 b- defN 23-Mar-19 08:44 deep_training/nlp/models/onerel_model.py
--rw-rw-rw-  2.0 fat     2735 b- defN 23-Apr-02 08:38 deep_training/nlp/models/pointer.py
--rw-rw-rw-  2.0 fat    13317 b- defN 23-Apr-02 08:38 deep_training/nlp/models/prefixtuning.py
--rw-rw-rw-  2.0 fat    15900 b- defN 23-Mar-19 08:44 deep_training/nlp/models/prgc_model.py
--rw-rw-rw-  2.0 fat    16100 b- defN 23-Mar-19 08:44 deep_training/nlp/models/promptbert_cse.py
--rw-rw-rw-  2.0 fat     5134 b- defN 23-Mar-19 08:44 deep_training/nlp/models/pure_model.py
--rw-rw-rw-  2.0 fat     3934 b- defN 23-Mar-19 08:44 deep_training/nlp/models/simcse.py
--rw-rw-rw-  2.0 fat     6007 b- defN 23-Apr-02 08:38 deep_training/nlp/models/span_ner.py
--rw-rw-rw-  2.0 fat    14439 b- defN 23-Mar-19 08:44 deep_training/nlp/models/spn4re.py
--rw-rw-rw-  2.0 fat    11368 b- defN 23-Mar-19 08:44 deep_training/nlp/models/tplinker.py
--rw-rw-rw-  2.0 fat     8142 b- defN 23-Mar-19 08:44 deep_training/nlp/models/tplinkerplus.py
--rw-rw-rw-  2.0 fat    31760 b- defN 23-Apr-03 13:31 deep_training/nlp/models/transformer.py
--rw-rw-rw-  2.0 fat     7953 b- defN 23-Mar-19 08:44 deep_training/nlp/models/tsdae_model.py
--rw-rw-rw-  2.0 fat     9025 b- defN 23-Apr-02 08:38 deep_training/nlp/models/w2ner.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-Mar-25 05:27 deep_training/nlp/models/LLaMA/__init__.py
--rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-19 08:44 deep_training/nlp/models/LLaMA/configuration.py
--rw-rw-rw-  2.0 fat    19183 b- defN 23-Mar-25 05:27 deep_training/nlp/models/LLaMA_parallel/__init__.py
--rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-19 08:44 deep_training/nlp/models/LLaMA_parallel/configuration.py
--rw-rw-rw-  2.0 fat    31627 b- defN 23-Mar-25 05:27 deep_training/nlp/models/PaLM/__init__.py
--rw-rw-rw-  2.0 fat     5890 b- defN 23-Mar-19 08:44 deep_training/nlp/models/PaLM/configuration.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-07 10:47 deep_training/nlp/models/adalora/__init__.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-07 10:47 deep_training/nlp/models/adalora/configuration.py
--rw-rw-rw-  2.0 fat    60192 b- defN 23-Apr-07 11:39 deep_training/nlp/models/chatglm/__init__.py
--rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-07 11:22 deep_training/nlp/models/chatglm/configuration.py
--rw-rw-rw-  2.0 fat    15150 b- defN 23-Apr-02 08:38 deep_training/nlp/models/chatglm/quantization.py
--rw-rw-rw-  2.0 fat    16460 b- defN 23-Apr-07 11:22 deep_training/nlp/models/chatglm/tokenization.py
--rw-rw-rw-  2.0 fat    34123 b- defN 23-Mar-25 05:27 deep_training/nlp/models/laMDA/__init__.py
--rw-rw-rw-  2.0 fat     5981 b- defN 23-Mar-19 08:44 deep_training/nlp/models/laMDA/configuration.py
--rw-rw-rw-  2.0 fat    13316 b- defN 23-Mar-25 05:27 deep_training/nlp/models/lora/__init__.py
--rw-rw-rw-  2.0 fat     7058 b- defN 23-Mar-19 08:44 deep_training/nlp/models/lora/configuration.py
--rw-rw-rw-  2.0 fat      102 b- defN 23-Mar-19 08:44 deep_training/nlp/models/splinker/__init__.py
--rw-rw-rw-  2.0 fat     2851 b- defN 23-Mar-19 08:44 deep_training/nlp/models/splinker/splinker.py
--rw-rw-rw-  2.0 fat    14478 b- defN 23-Mar-19 08:44 deep_training/nlp/models/t5decoder/__init__.py
--rw-rw-rw-  2.0 fat     6646 b- defN 23-Mar-19 08:44 deep_training/nlp/models/t5encoder/__init__.py
--rw-rw-rw-  2.0 fat       56 b- defN 23-Mar-19 08:44 deep_training/nlp/optimizer/__init__.py
--rw-rw-rw-  2.0 fat     5225 b- defN 23-Mar-19 08:44 deep_training/nlp/optimizer/lamb.py
--rw-rw-rw-  2.0 fat       99 b- defN 23-Mar-19 08:44 deep_training/nlp/optimizer/lion/__init__.py
--rw-rw-rw-  2.0 fat     2295 b- defN 23-Mar-19 08:44 deep_training/nlp/optimizer/lion/lion.py
--rw-rw-rw-  2.0 fat     2198 b- defN 23-Mar-19 08:44 deep_training/nlp/optimizer/lion/triton.py
--rw-rw-rw-  2.0 fat     2868 b- defN 23-Mar-19 08:44 deep_training/nlp/scheduler/__init__.py
--rw-rw-rw-  2.0 fat     6982 b- defN 23-Apr-02 08:38 deep_training/nlp/utils/__init__.py
--rw-rw-rw-  2.0 fat     6323 b- defN 23-Mar-19 08:44 deep_training/nlp/utils/adversarial.py
--rw-rw-rw-  2.0 fat    15256 b- defN 23-Mar-19 08:44 deep_training/nlp/utils/nlputils.py
--rw-rw-rw-  2.0 fat      795 b- defN 23-Mar-19 08:44 deep_training/nlp/utils/spearman.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/layers/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/losses/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/metrics/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/models/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/optimizer/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/scheduler/__init__.py
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-19 08:44 deep_training/tfnlp/utils/__init__.py
--rw-rw-rw-  2.0 fat       55 b- defN 23-Mar-19 08:44 deep_training/utils/__init__.py
--rw-rw-rw-  2.0 fat     1941 b- defN 23-Mar-19 08:44 deep_training/utils/distributed.py
--rw-rw-rw-  2.0 fat     1724 b- defN 23-Mar-19 08:44 deep_training/utils/func.py
--rw-rw-rw-  2.0 fat     5117 b- defN 23-Mar-19 08:44 deep_training/utils/maskedlm.py
--rw-rw-rw-  2.0 fat     7469 b- defN 23-Mar-19 08:44 deep_training/utils/trainer.py
--rw-rw-rw-  2.0 fat      603 b- defN 23-Apr-07 12:25 deep_training-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-07 12:25 deep_training-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-07 12:25 deep_training-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    13044 b- defN 23-Apr-07 12:25 deep_training-0.1.1.dist-info/RECORD
-136 files, 762842 bytes uncompressed, 202714 bytes compressed:  73.4%
+Zip file size: 243550 bytes, number of entries: 144
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-22 07:43 deep_training/__init__.py
+-rw-rw-rw-  2.0 fat      877 b- defN 23-Apr-11 03:08 deep_training/setup.py
+-rw-rw-rw-  2.0 fat       55 b- defN 22-Dec-09 05:30 deep_training/cv/__init__.py
+-rw-rw-rw-  2.0 fat      195 b- defN 23-Jan-29 01:07 deep_training/data_helper/__init__.py
+-rw-rw-rw-  2.0 fat    29088 b- defN 23-Apr-06 04:11 deep_training/data_helper/data_helper.py
+-rw-rw-rw-  2.0 fat     4926 b- defN 23-Feb-17 02:41 deep_training/data_helper/data_module.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Jan-29 01:07 deep_training/data_helper/data_writer.py
+-rw-rw-rw-  2.0 fat    12513 b- defN 23-Mar-27 00:33 deep_training/data_helper/training_args.py
+-rw-rw-rw-  2.0 fat       70 b- defN 22-Dec-13 03:17 deep_training/nlp/__init__.py
+-rw-rw-rw-  2.0 fat       56 b- defN 22-Nov-10 08:28 deep_training/nlp/layers/__init__.py
+-rw-rw-rw-  2.0 fat      241 b- defN 23-Mar-13 05:48 deep_training/nlp/layers/activate.py
+-rw-rw-rw-  2.0 fat    13271 b- defN 22-Nov-14 00:17 deep_training/nlp/layers/crf.py
+-rw-rw-rw-  2.0 fat     4653 b- defN 22-Dec-12 00:12 deep_training/nlp/layers/handshakingkernel.py
+-rw-rw-rw-  2.0 fat      435 b- defN 22-Dec-02 00:22 deep_training/nlp/layers/mask.py
+-rw-rw-rw-  2.0 fat     1319 b- defN 22-Dec-12 00:12 deep_training/nlp/layers/mhslayer.py
+-rw-rw-rw-  2.0 fat     5911 b- defN 22-Dec-08 00:08 deep_training/nlp/layers/norm.py
+-rw-rw-rw-  2.0 fat     1220 b- defN 22-Jul-21 00:57 deep_training/nlp/layers/prefix_encoder.py
+-rw-rw-rw-  2.0 fat     7259 b- defN 22-Dec-14 02:36 deep_training/nlp/layers/seq_pointer.py
+-rw-rw-rw-  2.0 fat     3550 b- defN 22-Dec-15 00:57 deep_training/nlp/layers/w2ner.py
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v1/__init__.py
+-rw-rw-rw-  2.0 fat    15095 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v1/layers.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v1/utils.py
+-rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v2/__init__.py
+-rw-rw-rw-  2.0 fat    15311 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v2/adalora.py
+-rw-rw-rw-  2.0 fat     8488 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v2/layers.py
+-rw-rw-rw-  2.0 fat     9106 b- defN 23-Apr-11 00:30 deep_training/nlp/layers/lora_v2/utils.py
+-rw-rw-rw-  2.0 fat     3662 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchAllTripletLoss.py
+-rw-rw-rw-  2.0 fat     3880 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
+-rw-rw-rw-  2.0 fat     8358 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchHardTripletLoss.py
+-rw-rw-rw-  2.0 fat     4552 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchSemiHardTripletLoss.py
+-rw-rw-rw-  2.0 fat     2255 b- defN 22-Nov-18 01:05 deep_training/nlp/losses/ContrastiveLoss.py
+-rw-rw-rw-  2.0 fat     4573 b- defN 22-Nov-16 07:04 deep_training/nlp/losses/ContrastiveTensionLoss.py
+-rw-rw-rw-  2.0 fat     1359 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/CosineSimilarityLoss.py
+-rw-rw-rw-  2.0 fat      742 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/MSELoss.py
+-rw-rw-rw-  2.0 fat     1315 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/MarginMSELoss.py
+-rw-rw-rw-  2.0 fat     5302 b- defN 22-Nov-16 07:11 deep_training/nlp/losses/MegaBatchMarginLoss.py
+-rw-rw-rw-  2.0 fat     2420 b- defN 23-Jan-18 08:08 deep_training/nlp/losses/MultipleNegativesRankingLoss.py
+-rw-rw-rw-  2.0 fat     2905 b- defN 22-Nov-16 07:11 deep_training/nlp/losses/MultipleNegativesSymmetricRankingLoss.py
+-rw-rw-rw-  2.0 fat     1863 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/OnlineContrastiveLoss.py
+-rw-rw-rw-  2.0 fat     2880 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/SoftmaxLoss.py
+-rw-rw-rw-  2.0 fat     2306 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/TripletLoss.py
+-rw-rw-rw-  2.0 fat      599 b- defN 22-Nov-17 00:20 deep_training/nlp/losses/__init__.py
+-rw-rw-rw-  2.0 fat      661 b- defN 22-Dec-02 08:50 deep_training/nlp/losses/bce_loss.py
+-rw-rw-rw-  2.0 fat     1397 b- defN 22-Nov-17 05:38 deep_training/nlp/losses/center_loss.py
+-rw-rw-rw-  2.0 fat     1772 b- defN 22-Nov-17 07:28 deep_training/nlp/losses/circle_loss.py
+-rw-rw-rw-  2.0 fat     1056 b- defN 23-Jan-13 07:26 deep_training/nlp/losses/contrast.py
+-rw-rw-rw-  2.0 fat      619 b- defN 22-Aug-22 01:11 deep_training/nlp/losses/dice_loss.py
+-rw-rw-rw-  2.0 fat      710 b- defN 22-Nov-16 06:49 deep_training/nlp/losses/focal_loss.py
+-rw-rw-rw-  2.0 fat      882 b- defN 22-Aug-22 01:11 deep_training/nlp/losses/label_smoothing.py
+-rw-rw-rw-  2.0 fat      547 b- defN 23-Jan-29 01:07 deep_training/nlp/losses/lm_loss.py
+-rw-rw-rw-  2.0 fat     2149 b- defN 22-Dec-29 06:05 deep_training/nlp/losses/loss_arcface.py
+-rw-rw-rw-  2.0 fat      962 b- defN 22-Dec-05 00:45 deep_training/nlp/losses/loss_casrel.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 22-Dec-21 00:45 deep_training/nlp/losses/loss_cosent.py
+-rw-rw-rw-  2.0 fat     1912 b- defN 22-Dec-29 06:03 deep_training/nlp/losses/loss_cosface.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 22-Dec-08 00:49 deep_training/nlp/losses/loss_globalpointer.py
+-rw-rw-rw-  2.0 fat     6020 b- defN 23-Jan-09 00:29 deep_training/nlp/losses/loss_infonce.py
+-rw-rw-rw-  2.0 fat      884 b- defN 22-Dec-23 00:05 deep_training/nlp/losses/loss_kl.py
+-rw-rw-rw-  2.0 fat     1270 b- defN 23-Mar-14 03:03 deep_training/nlp/losses/loss_mhslinker.py
+-rw-rw-rw-  2.0 fat      617 b- defN 22-Dec-14 08:37 deep_training/nlp/losses/loss_r-drop.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 22-Dec-29 06:04 deep_training/nlp/losses/loss_sphereface.py
+-rw-rw-rw-  2.0 fat      562 b- defN 22-Nov-25 06:44 deep_training/nlp/losses/loss_splinker.py
+-rw-rw-rw-  2.0 fat    10822 b- defN 23-Jan-09 09:00 deep_training/nlp/losses/loss_spn4re.py
+-rw-rw-rw-  2.0 fat     5644 b- defN 22-Dec-12 00:12 deep_training/nlp/losses/loss_tplinker.py
+-rw-rw-rw-  2.0 fat     2466 b- defN 23-Jan-18 09:12 deep_training/nlp/losses/utils.py
+-rw-rw-rw-  2.0 fat       71 b- defN 22-Dec-13 03:17 deep_training/nlp/metrics/__init__.py
+-rw-rw-rw-  2.0 fat      655 b- defN 22-Dec-02 00:22 deep_training/nlp/metrics/pointer.py
+-rw-rw-rw-  2.0 fat       58 b- defN 22-Nov-22 08:00 deep_training/nlp/models/__init__.py
+-rw-rw-rw-  2.0 fat     6811 b- defN 22-Dec-23 00:05 deep_training/nlp/models/casrel.py
+-rw-rw-rw-  2.0 fat     5078 b- defN 22-Dec-22 08:21 deep_training/nlp/models/crf_cascad.py
+-rw-rw-rw-  2.0 fat     1573 b- defN 22-Dec-22 08:21 deep_training/nlp/models/crf_model.py
+-rw-rw-rw-  2.0 fat    12970 b- defN 23-Jan-18 06:52 deep_training/nlp/models/diffcse.py
+-rw-rw-rw-  2.0 fat     5388 b- defN 23-Mar-30 00:20 deep_training/nlp/models/esimcse.py
+-rw-rw-rw-  2.0 fat     4194 b- defN 23-Mar-09 01:21 deep_training/nlp/models/gec_model.py
+-rw-rw-rw-  2.0 fat    10824 b- defN 22-Dec-26 02:03 deep_training/nlp/models/gplinker.py
+-rw-rw-rw-  2.0 fat     3799 b- defN 23-Jan-17 08:25 deep_training/nlp/models/infonce.py
+-rw-rw-rw-  2.0 fat     2444 b- defN 22-Dec-22 08:21 deep_training/nlp/models/mhs_ner.py
+-rw-rw-rw-  2.0 fat     5976 b- defN 22-Dec-22 08:21 deep_training/nlp/models/mhslinker.py
+-rw-rw-rw-  2.0 fat     4646 b- defN 23-Jan-18 06:52 deep_training/nlp/models/onerel_model.py
+-rw-rw-rw-  2.0 fat     2735 b- defN 23-Apr-03 00:32 deep_training/nlp/models/pointer.py
+-rw-rw-rw-  2.0 fat    13317 b- defN 23-Apr-03 00:32 deep_training/nlp/models/prefixtuning.py
+-rw-rw-rw-  2.0 fat    15900 b- defN 23-Jan-18 06:52 deep_training/nlp/models/prgc_model.py
+-rw-rw-rw-  2.0 fat    16100 b- defN 23-Jan-29 01:07 deep_training/nlp/models/promptbert_cse.py
+-rw-rw-rw-  2.0 fat     5134 b- defN 23-Jan-18 06:52 deep_training/nlp/models/pure_model.py
+-rw-rw-rw-  2.0 fat     3934 b- defN 23-Jan-16 07:30 deep_training/nlp/models/simcse.py
+-rw-rw-rw-  2.0 fat     6007 b- defN 23-Apr-03 00:32 deep_training/nlp/models/span_ner.py
+-rw-rw-rw-  2.0 fat    14439 b- defN 23-Jan-18 06:52 deep_training/nlp/models/spn4re.py
+-rw-rw-rw-  2.0 fat    11368 b- defN 22-Dec-22 08:17 deep_training/nlp/models/tplinker.py
+-rw-rw-rw-  2.0 fat     8142 b- defN 22-Dec-22 08:17 deep_training/nlp/models/tplinkerplus.py
+-rw-rw-rw-  2.0 fat    31760 b- defN 23-Apr-04 00:31 deep_training/nlp/models/transformer.py
+-rw-rw-rw-  2.0 fat     7953 b- defN 23-Jan-15 03:09 deep_training/nlp/models/tsdae_model.py
+-rw-rw-rw-  2.0 fat     9025 b- defN 23-Apr-03 00:32 deep_training/nlp/models/w2ner.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-Mar-27 00:33 deep_training/nlp/models/LLaMA/__init__.py
+-rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-13 01:04 deep_training/nlp/models/LLaMA/configuration.py
+-rw-rw-rw-  2.0 fat    19183 b- defN 23-Mar-27 00:33 deep_training/nlp/models/LLaMA_parallel/__init__.py
+-rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-10 00:30 deep_training/nlp/models/LLaMA_parallel/configuration.py
+-rw-rw-rw-  2.0 fat    31627 b- defN 23-Mar-13 06:15 deep_training/nlp/models/PaLM/__init__.py
+-rw-rw-rw-  2.0 fat     5890 b- defN 23-Mar-13 06:15 deep_training/nlp/models/PaLM/configuration.py
+-rw-rw-rw-  2.0 fat    60188 b- defN 23-Apr-10 00:42 deep_training/nlp/models/chatglm/__init__.py
+-rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-10 00:42 deep_training/nlp/models/chatglm/configuration.py
+-rw-rw-rw-  2.0 fat    15150 b- defN 23-Apr-03 00:32 deep_training/nlp/models/chatglm/quantization.py
+-rw-rw-rw-  2.0 fat    16460 b- defN 23-Apr-10 00:42 deep_training/nlp/models/chatglm/tokenization.py
+-rw-rw-rw-  2.0 fat    34123 b- defN 23-Mar-13 06:18 deep_training/nlp/models/laMDA/__init__.py
+-rw-rw-rw-  2.0 fat     5981 b- defN 23-Mar-13 06:15 deep_training/nlp/models/laMDA/configuration.py
+-rw-rw-rw-  2.0 fat       44 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/__init__.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v1/__init__.py
+-rw-rw-rw-  2.0 fat     7054 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v1/configuration.py
+-rw-rw-rw-  2.0 fat    13385 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v1/lora_wrapper.py
+-rw-rw-rw-  2.0 fat      206 b- defN 23-Apr-11 01:58 deep_training/nlp/models/lora/v2/__init__.py
+-rw-rw-rw-  2.0 fat    13112 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/adalora_model.py
+-rw-rw-rw-  2.0 fat    10797 b- defN 23-Apr-11 02:38 deep_training/nlp/models/lora/v2/configuration.py
+-rw-rw-rw-  2.0 fat    10398 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/lora_model.py
+-rw-rw-rw-  2.0 fat    10265 b- defN 23-Apr-11 01:58 deep_training/nlp/models/lora/v2/lora_wrapper.py
+-rw-rw-rw-  2.0 fat     4889 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/save_and_load.py
+-rw-rw-rw-  2.0 fat      102 b- defN 22-Nov-22 08:00 deep_training/nlp/models/splinker/__init__.py
+-rw-rw-rw-  2.0 fat     2851 b- defN 22-Dec-22 08:14 deep_training/nlp/models/splinker/splinker.py
+-rw-rw-rw-  2.0 fat    14478 b- defN 23-Feb-11 09:07 deep_training/nlp/models/t5decoder/__init__.py
+-rw-rw-rw-  2.0 fat     6646 b- defN 23-Feb-09 00:28 deep_training/nlp/models/t5encoder/__init__.py
+-rw-rw-rw-  2.0 fat       56 b- defN 22-Dec-14 08:02 deep_training/nlp/optimizer/__init__.py
+-rw-rw-rw-  2.0 fat     5225 b- defN 23-Mar-08 00:14 deep_training/nlp/optimizer/lamb.py
+-rw-rw-rw-  2.0 fat       99 b- defN 23-Mar-02 05:27 deep_training/nlp/optimizer/lion/__init__.py
+-rw-rw-rw-  2.0 fat     2295 b- defN 23-Mar-02 05:27 deep_training/nlp/optimizer/lion/lion.py
+-rw-rw-rw-  2.0 fat     2198 b- defN 23-Mar-02 05:27 deep_training/nlp/optimizer/lion/triton.py
+-rw-rw-rw-  2.0 fat     2868 b- defN 22-Dec-14 08:00 deep_training/nlp/scheduler/__init__.py
+-rw-rw-rw-  2.0 fat     6982 b- defN 23-Apr-03 00:32 deep_training/nlp/utils/__init__.py
+-rw-rw-rw-  2.0 fat     6323 b- defN 23-Jan-29 01:07 deep_training/nlp/utils/adversarial.py
+-rw-rw-rw-  2.0 fat    15256 b- defN 23-Jan-03 01:54 deep_training/nlp/utils/nlputils.py
+-rw-rw-rw-  2.0 fat      795 b- defN 23-Jan-11 07:02 deep_training/nlp/utils/spearman.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/layers/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/losses/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/metrics/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/models/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/optimizer/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/scheduler/__init__.py
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:26 deep_training/tfnlp/utils/__init__.py
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Mar-07 01:20 deep_training/utils/__init__.py
+-rw-rw-rw-  2.0 fat     1941 b- defN 23-Mar-07 01:20 deep_training/utils/distributed.py
+-rw-rw-rw-  2.0 fat     1724 b- defN 23-Mar-07 01:22 deep_training/utils/func.py
+-rw-rw-rw-  2.0 fat     5117 b- defN 23-Feb-21 09:01 deep_training/utils/maskedlm.py
+-rw-rw-rw-  2.0 fat     7469 b- defN 23-Mar-20 00:27 deep_training/utils/trainer.py
+-rw-rw-rw-  2.0 fat      626 b- defN 23-Apr-11 03:09 deep_training-0.1.2rc0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 03:09 deep_training-0.1.2rc0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Apr-11 03:09 deep_training-0.1.2rc0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    13896 b- defN 23-Apr-11 03:09 deep_training-0.1.2rc0.dist-info/RECORD
+144 files, 831287 bytes uncompressed, 221026 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -51,27 +51,33 @@
 
 Filename: deep_training/nlp/layers/seq_pointer.py
 Comment: 
 
 Filename: deep_training/nlp/layers/w2ner.py
 Comment: 
 
-Filename: deep_training/nlp/layers/adalora/__init__.py
+Filename: deep_training/nlp/layers/lora_v1/__init__.py
 Comment: 
 
-Filename: deep_training/nlp/layers/adalora/layers.py
+Filename: deep_training/nlp/layers/lora_v1/layers.py
 Comment: 
 
-Filename: deep_training/nlp/layers/lora/__init__.py
+Filename: deep_training/nlp/layers/lora_v1/utils.py
 Comment: 
 
-Filename: deep_training/nlp/layers/lora/layers.py
+Filename: deep_training/nlp/layers/lora_v2/__init__.py
 Comment: 
 
-Filename: deep_training/nlp/layers/lora/utils.py
+Filename: deep_training/nlp/layers/lora_v2/adalora.py
+Comment: 
+
+Filename: deep_training/nlp/layers/lora_v2/layers.py
+Comment: 
+
+Filename: deep_training/nlp/layers/lora_v2/utils.py
 Comment: 
 
 Filename: deep_training/nlp/losses/BatchAllTripletLoss.py
 Comment: 
 
 Filename: deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
 Comment: 
@@ -279,20 +285,14 @@
 
 Filename: deep_training/nlp/models/PaLM/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/PaLM/configuration.py
 Comment: 
 
-Filename: deep_training/nlp/models/adalora/__init__.py
-Comment: 
-
-Filename: deep_training/nlp/models/adalora/configuration.py
-Comment: 
-
 Filename: deep_training/nlp/models/chatglm/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/chatglm/configuration.py
 Comment: 
 
 Filename: deep_training/nlp/models/chatglm/quantization.py
@@ -306,15 +306,39 @@
 
 Filename: deep_training/nlp/models/laMDA/configuration.py
 Comment: 
 
 Filename: deep_training/nlp/models/lora/__init__.py
 Comment: 
 
-Filename: deep_training/nlp/models/lora/configuration.py
+Filename: deep_training/nlp/models/lora/v1/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v1/configuration.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v1/lora_wrapper.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/adalora_model.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/configuration.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/lora_model.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/lora_wrapper.py
+Comment: 
+
+Filename: deep_training/nlp/models/lora/v2/save_and_load.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/splinker.py
 Comment: 
@@ -390,20 +414,20 @@
 
 Filename: deep_training/utils/maskedlm.py
 Comment: 
 
 Filename: deep_training/utils/trainer.py
 Comment: 
 
-Filename: deep_training-0.1.1.dist-info/METADATA
+Filename: deep_training-0.1.2rc0.dist-info/METADATA
 Comment: 
 
-Filename: deep_training-0.1.1.dist-info/WHEEL
+Filename: deep_training-0.1.2rc0.dist-info/WHEEL
 Comment: 
 
-Filename: deep_training-0.1.1.dist-info/top_level.txt
+Filename: deep_training-0.1.2rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: deep_training-0.1.1.dist-info/RECORD
+Filename: deep_training-0.1.2rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deep_training/setup.py

```diff
@@ -1,15 +1,15 @@
 #! -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 ignore = ['test','tests']
 setup(
     name='deep_training',
-    version='0.1.1',
+    version='0.1.2rc0',
     description='an easy training architecture',
     long_description='torch_training: https://github.com/ssbuild/deep_training.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/deep_training',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=['pytorch-lightning>=2',
```

## deep_training/nlp/models/chatglm/__init__.py

```diff
@@ -45,15 +45,15 @@
 ]
 
 
 class InvalidScoreLogitsProcessor(LogitsProcessor):
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor) -> torch.FloatTensor:
         if torch.isnan(scores).any() or torch.isinf(scores).any():
             scores.zero_()
-            scores[..., 20005] = 5e4
+            scores[..., 5] = 5e4
         return scores
```

## deep_training/nlp/models/lora/__init__.py

```diff
@@ -1,296 +1,2 @@
 # @Time    : 2023/3/2 20:55
-# @Author  : tk
-# @FileName: __init__.py.py
-import os
-import re
-import warnings
-from contextlib import contextmanager
-from dataclasses import asdict, dataclass, field
-from enum import Enum
-from typing import Optional, Union, List
-
-import torch
-from transformers import Conv1D
-from transformers.utils import PushToHubMixin
-
-from .configuration import LoraArguments, WEIGHTS_NAME
-from ...layers.lora.layers import MergedLinear, is_bnb_available, LoraLayer, Linear
-from ...layers.lora.utils import mark_only_lora_as_trainable
-
-__all__ = [
-    'LoraArguments',
-    'LoraModel',
-    'LoraLayer'
-]
-
-if is_bnb_available():
-    import bitsandbytes as bnb
-    from ...layers.lora.layers import  Linear8bitLt
-
-
-
-
-
-def get_lora_model_state_dict(model, state_dict=None):
-    """
-    Get the state dict of the Lora model.
-
-    Args:
-        model ([`LoraModel`]): The Lora model. When using torch.nn.DistributedDataParallel, DeepSpeed or FSDP,
-        the model should be the underlying model/unwrapped model (i.e. model.module).
-        state_dict (`dict`, *optional*, defaults to `None`):
-            The state dict of the model. If not provided, the state dict of the model
-        will be used.
-    """
-    if state_dict is None:
-        state_dict = model.state_dict()
-
-    # to_return = lora_state_dict(model, bias=model.lora_config.bias)
-    # adapted from `https://github.com/microsoft/LoRA/blob/main/loralib/utils.py`
-    # to directly with the state dict which is necessary when using DeepSpeed or FSDP
-    bias = model.lora_config.bias
-    if bias == "none":
-        to_return = {k: state_dict[k] for k in state_dict if "lora_" in k}
-    elif bias == "all":
-        to_return = {k: state_dict[k] for k in state_dict if "lora_" in k or "bias" in k}
-    elif bias == "lora_only":
-        to_return = {}
-        for k in state_dict:
-            if "lora_" in k:
-                to_return[k] = state_dict[k]
-                bias_name = k.split("lora_")[0] + "bias"
-                if bias_name in state_dict:
-                    to_return[bias_name] = state_dict[bias_name]
-    else:
-        raise NotImplementedError
-
-    if model.modules_to_save is not None:
-        for key, value in state_dict.items():
-            if any(module_name in key for module_name in model.modules_to_save):
-                to_return[key] = value
-    return to_return
-
-
-def set_lora_model_state_dict(model, lora_model_state_dict):
-    """
-    Set the state dict of the Lora model.
-
-    Args:
-        model ([`LoraModel`]): The Lora model.
-        lora_model_state_dict (`dict`): The state dict of the Lora model.
-    """
-
-    model.load_state_dict(lora_model_state_dict, strict=False)
-    return model
-
-
-
-class LoraModel(torch.nn.Module,PushToHubMixin):
-    def __init__(self, model, config):
-        torch.nn.Module.__init__(self)
-        PushToHubMixin.__init__(self)
-        self.lora_config = config
-        self.model = model
-        self._find_and_replace()
-        mark_only_lora_as_trainable(self.model, self.lora_config.bias)
-        self.forward = self.model.forward
-
-    def _find_and_replace(self):
-        loaded_in_8bit = getattr(self.model, "is_loaded_in_8bit", False)
-        if loaded_in_8bit and not is_bnb_available():
-            raise ImportError(
-                "To use Lora with 8-bit quantization, please install the `bitsandbytes` package. "
-                "You can install it with `pip install bitsandbytes`."
-            )
-        is_target_modules_in_base_model = False
-        kwargs = {
-            "r": self.lora_config.r,
-            "lora_alpha": self.lora_config.lora_alpha,
-            "lora_dropout": self.lora_config.lora_dropout,
-            "fan_in_fan_out": self.lora_config.fan_in_fan_out,
-            "merge_weights": self.lora_config.merge_weights or self.lora_config.inference_mode,
-        }
-
-        if self.lora_config.target_dtype is not None:
-            if self.lora_config.target_dtype == 16 or self.lora_config.target_dtype == '16':
-                kwargs['dtype'] = torch.float16
-            elif self.lora_config.target_dtype == 32 or self.lora_config.target_dtype == '32':
-                kwargs['dtype'] = torch.float32
-            elif self.lora_config.target_dtype == 64 or self.lora_config.target_dtype == '64':
-                kwargs['dtype'] = torch.float64
-            elif self.lora_config.target_dtype == 'bf16':
-                kwargs['dtype'] = torch.bfloat16
-            elif isinstance(self.lora_config.target_dtype,torch.dtype):
-                kwargs['dtype'] = self.lora_config.target_dtype
-
-        key_list = [key for key, _ in self.model.named_modules()]
-        for key in key_list:
-            if isinstance(self.lora_config.target_modules, str):
-                target_module_found = re.fullmatch(self.lora_config.target_modules, key)
-            else:
-                target_module_found = any(key.endswith(target_key) for target_key in self.lora_config.target_modules)
-            if target_module_found:
-                if not is_target_modules_in_base_model:
-                    is_target_modules_in_base_model = True
-                parent, target, target_name = self._get_submodules(key)
-                bias = target.bias is not None
-                if loaded_in_8bit and isinstance(target, bnb.nn.Linear8bitLt) and self.lora_config.enable_lora is None:
-                    kwargs.update(
-                        {
-                            "has_fp16_weights": target.state.has_fp16_weights,
-                            "memory_efficient_backward": target.state.memory_efficient_backward,
-                            "threshold": target.state.threshold,
-                            "index": target.index,
-                        }
-                    )
-                    new_module = Linear8bitLt(target.in_features, target.out_features, bias=bias, **kwargs)
-                elif isinstance(target, torch.nn.Linear) and self.lora_config.enable_lora is None:
-                    new_module = Linear(target.in_features, target.out_features, bias=bias, **kwargs)
-                elif self.lora_config.enable_lora is not None:
-                    kwargs.update({"enable_lora": self.lora_config.enable_lora})
-                    if isinstance(target, Conv1D):
-                        in_features, out_features = target.weight.shape
-                    else:
-                        in_features, out_features = target.in_features, target.out_features
-                        if kwargs["fan_in_fan_out"]:
-                            warnings.warn(
-                                "fan_in_fan_out is set to True but the target module is not a Conv1D. "
-                                "Setting fan_in_fan_out to False."
-                            )
-                            kwargs["fan_in_fan_out"] = False
-                    new_module = MergedLinear(in_features, out_features, bias=bias, **kwargs)
-                self._replace_module(parent, target_name, new_module, target)
-        if not is_target_modules_in_base_model:
-            raise ValueError(
-                f"Target modules {self.lora_config.target_modules} not found in the base model. "
-                f"Please check the target modules and try again."
-            )
-
-    def _get_submodules(self, key):
-        parent = self.model.get_submodule(".".join(key.split(".")[:-1]))
-        target_name = key.split(".")[-1]
-        target = self.model.get_submodule(key)
-        return parent, target, target_name
-
-    def _replace_module(self, parent_module, child_name, new_module, old_module):
-        setattr(parent_module, child_name, new_module)
-        new_module.weight = old_module.weight
-        if old_module.bias is not None:
-            new_module.bias = old_module.bias
-        if getattr(old_module, "state", None) is not None:
-            new_module.state = old_module.state
-            new_module.to(old_module.weight.device)
-
-    def __getattr__(self, name: str):
-        """Forward missing attributes to the wrapped module."""
-        try:
-            return super().__getattr__(name)  # defer to nn.Module's logic
-        except AttributeError:
-            return getattr(self.model, name)
-
-    @property
-    def modules_to_save(self):
-        return None
-
-    def get_lora_config_as_dict(self, inference: bool = False):
-        config = {k: v.value if isinstance(v, Enum) else v for k, v in asdict(self.lora_config).items()}
-        if inference:
-            config["inference_mode"] = True
-        return config
-
-    def _set_adapter_layers(self, enabled=True):
-        for module in self.model.modules():
-            if isinstance(module, LoraLayer):
-                module.disable_adapters = False if enabled else True
-
-    def enable_adapter_layers(self):
-        self._set_adapter_layers(enabled=True)
-
-    def disable_adapter_layers(self):
-        self._set_adapter_layers(enabled=False)
-
-    def save_pretrained(self, save_directory, **kwargs):
-        r"""
-        Args:
-        This function saves the adapter model and the adapter configuration files to a directory, so that it can be
-        re-loaded using the `LoraModel.from_pretrained` class method, and also used by the `LoraModel.push_to_hub`
-        method.
-            save_directory (`str`):
-                Directory where the adapter model and configuration files will be saved (will be created if it does not
-                exist).
-            **kwargs:
-                Additional keyword arguments passed along to the `push_to_hub` method.
-        """
-        if os.path.isfile(save_directory):
-            raise ValueError(f"Provided path ({save_directory}) should be a directory, not a file")
-        os.makedirs(save_directory, exist_ok=True)
-
-        # save only the trainable weights
-        output_state_dict = get_lora_model_state_dict(self, kwargs.get("state_dict", None))
-        torch.save(output_state_dict, os.path.join(save_directory, WEIGHTS_NAME))
-
-        # save the config and change the inference mode to `True`
-        inference_mode = self.lora_config.inference_mode
-        self.lora_config.inference_mode = True
-        self.lora_config.save_pretrained(save_directory)
-        self.lora_config.inference_mode = inference_mode
-
-    @classmethod
-    def from_pretrained(cls, model, pretrained_model_name_or_path,lora_config: LoraArguments = None, **kwargs):
-        r"""
-        Args:
-        Instantiate a `LoraModel` from a pretrained Lora configuration and weights.
-            model (`transformers.PreTrainedModel`):
-                The model to be adapted. The model should be initialized with the `from_pretrained` method. from
-                `transformers` library.
-            model_id (`str`):
-                The name of the Lora configuration to use. Can be either:
-                    - A string, the `model id` of a Lora configuration hosted inside a model repo on
-                        huggingface Hub
-                    - A path to a directory containing a Lora configuration file saved using the
-                        `save_pretrained` method, e.g., ``./my_lora_config_directory/``.
-        """
-        if lora_config is None:
-            lora_config: LoraArguments = LoraArguments.from_pretrained(pretrained_model_name_or_path)
-
-        model = cls(model, lora_config)
-        # load weights if any
-        if os.path.exists(os.path.join(pretrained_model_name_or_path, WEIGHTS_NAME)):
-            filename = os.path.join(pretrained_model_name_or_path, WEIGHTS_NAME)
-        else:
-            raise ValueError(
-                f"Can't find weights for {pretrained_model_name_or_path} in {pretrained_model_name_or_path} or in the Hugging Face Hub. "
-                f"Please check that the file {WEIGHTS_NAME} is present at {pretrained_model_name_or_path}."
-            )
-
-        adapters_weights = torch.load(
-            filename, map_location=torch.device("cuda" if torch.cuda.is_available() else "cpu"))
-        # load the weights into the model
-        model = set_lora_model_state_dict(model, adapters_weights)
-        return model
-
-    def print_trainable_parameters(self):
-        """
-        Prints the number of trainable parameters in the model.
-        """
-        trainable_params = 0
-        all_param = 0
-        for _, param in self.named_parameters():
-            num_params = param.numel()
-            # if using DS Zero 3 and the weights are initialized empty
-            if num_params == 0 and hasattr(param, "ds_numel"):
-                num_params = param.ds_numel
-
-            all_param += num_params
-            if param.requires_grad:
-                trainable_params += param.numel()
-        print(
-            f"trainable params: {trainable_params} || all params: {all_param} || trainable%: {100 * trainable_params / all_param}"
-        )
-
-    def __getattr__(self, name: str):
-        """Forward missing attributes to the wrapped module."""
-        try:
-            return super().__getattr__(name)  # defer to nn.Module's logic
-        except AttributeError:
-            return getattr(self.model, name)
+# @Author  : tk
```

## Comparing `deep_training/nlp/layers/adalora/layers.py` & `deep_training/nlp/layers/lora_v2/adalora.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-# -*- coding: utf-8 -*-
-# @Time    : 2023/4/7 16:07
+# @Time    : 2023/4/7 23:25
+# @Author  : tk
+# @FileName: adalora
+import warnings
 
 import torch
 from torch import nn
-from ..lora.layers import LoraLayer
+from torch.nn import functional as F
+from .layers import LoraLayer,is_bnb_available
+from .utils import transpose
+
+if is_bnb_available():
+    import bitsandbytes as bnb
 
 class AdaLoraLayer(LoraLayer):
     def __init__(
         self,
         in_features: int,
         out_features: int,
     ):
```

## Comparing `deep_training/nlp/layers/lora/layers.py` & `deep_training/nlp/layers/lora_v1/layers.py`

 * *Files identical despite different names*

## Comparing `deep_training/nlp/layers/lora/utils.py` & `deep_training/nlp/layers/lora_v1/utils.py`

 * *Files identical despite different names*

## Comparing `deep_training/nlp/models/lora/configuration.py` & `deep_training/nlp/models/lora/v1/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # @Time    : 2023/3/2 20:55
 # @Author  : tk
 # @FileName: config.py
 import json
 import os
 from dataclasses import dataclass, field, asdict
 from typing import Union, Optional, List, Literal, AnyStr
-
 from transformers.utils import PushToHubMixin
 
 WEIGHTS_NAME = "adapter_model.bin"
 CONFIG_NAME = "adapter_config.json"
 
 _PRECISION_INPUT_INT = Literal[64, 32, 16]
 _PRECISION_INPUT_STR = Literal["64", "32", "16", "bf16"]
@@ -118,15 +117,14 @@
         enable_lora ( `List[bool]`): Used with `lora.MergedLinear`.
         bias (`str`): Bias type for Lora. Can be 'none', 'all' or 'lora_only'
         modules_to_save (`List[str]`):List of modules apart from LoRA layers to be set as trainable
             and saved in the final checkpoint.
     """
     lora_model_name_or_path: str = field(default=None, metadata={"help": "The name of the base model to use."})
     inference_mode: bool = field(default=False, metadata={"help": "Whether to use inference mode"})
-
     with_lora: bool = field(default=False, metadata={"help": "whether use lora"})
     r: int = field(default=8, metadata={"help": "Lora attention dimension"})
     target_modules: Optional[Union[List[str], str]] = field(
         default=None,
         metadata={
             "help": "List of module names or regex expression of the module names to replace with Lora."
                     "For example, ['q', 'v'] or '.*decoder.*(SelfAttention|EncDecAttention).*(q|v)$' "
```

## Comparing `deep_training-0.1.1.dist-info/METADATA` & `deep_training-0.1.2rc0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: deep-training
-Version: 0.1.1
+Version: 0.1.2rc0
 Summary: an easy training architecture
 Home-page: https://github.com/ssbuild/deep_training
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: Apache License 2.0
+Platform: UNKNOWN
 Requires-Dist: pytorch-lightning (>=2)
 Requires-Dist: fastdatasets (<=1,>=0.9.6)
 Requires-Dist: tfrecords (<=1,>=0.2.4)
 Requires-Dist: sentencepiece
 Requires-Dist: numpy
 Requires-Dist: transformers (>=4.22)
 Requires-Dist: seqmetric
 Requires-Dist: scipy
 Requires-Dist: scikit-learn
 Requires-Dist: tqdm
 Requires-Dist: six
 
 torch_training: https://github.com/ssbuild/deep_training.git
+
+
```

## Comparing `deep_training-0.1.1.dist-info/RECORD` & `deep_training-0.1.2rc0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 deep_training/__init__.py,sha256=bhATnUT4VEzwvA8_8IwxspnDRKf32ZgEeHYCN2E5Dd4,47
-deep_training/setup.py,sha256=LxwOOAHGxZMcejSZ_B_yO6-qv3HI5R9n3SYDJTI9W_U,874
+deep_training/setup.py,sha256=YuxYG7ftu-my5yz5hTKDfznZnsXnsnf6T4wX7kLdWVQ,877
 deep_training/cv/__init__.py,sha256=J-zlKxMsAfAgoO0vSAzgYJXSuMSJcJ7NKAPKeaeC3TM,55
 deep_training/data_helper/__init__.py,sha256=P8rAMalR6xNepAf-9ldGoOSsEiUtur8Px6gUpTXQhd8,195
 deep_training/data_helper/data_helper.py,sha256=wamHVXHpCIcG-COkVLRmwIjmcQ0MQy99xjago0ulkkY,29088
 deep_training/data_helper/data_module.py,sha256=cRqwzcKMpFaE2HhdbAEwrIC9KxOE0rLkeQ25VCJh2W8,4926
 deep_training/data_helper/data_writer.py,sha256=BnxUmMuR60Wawd1SH9TTEBsQuDLozxWJdmLozuO-Wv4,1383
 deep_training/data_helper/training_args.py,sha256=VOHdJafXr8DIGOF50xuD62Nv2ZeLvdZQR9jE6qfhpb8,12513
 deep_training/nlp/__init__.py,sha256=L4_ltrwpG8mrgN1hZRKimefLHgjhRYyXVtLMFzr1grw,70
@@ -13,19 +13,21 @@
 deep_training/nlp/layers/handshakingkernel.py,sha256=BRJZbEjKM347q8zEMEtJXxXjmqhegmQgqebhqMy4UkI,4653
 deep_training/nlp/layers/mask.py,sha256=8SB_Hl9X48-yuJMCPjLDabDXvgWvH4VPqUOSVDmePFs,435
 deep_training/nlp/layers/mhslayer.py,sha256=Ky6xW3hNe0x4WWPPoWa8pZkCp_-MR5VE0yKHYPzzpd0,1319
 deep_training/nlp/layers/norm.py,sha256=r_yHSnDAv8RY1nb1VS1lMWttbJVyCO376OIuu0So8c8,5911
 deep_training/nlp/layers/prefix_encoder.py,sha256=y_Y4wWLnEyZJf33pQJFjWfl-AX1VS8Aejj3JXOdiRXQ,1220
 deep_training/nlp/layers/seq_pointer.py,sha256=KmwZclK9gqdluy2o-h7nd3zL3EZjjjw1L6dz0isCFI8,7259
 deep_training/nlp/layers/w2ner.py,sha256=fP7hlMHp1NTH6elNMJA-wBOER76VTouSSsKCinLsCyM,3550
-deep_training/nlp/layers/adalora/__init__.py,sha256=yP4EglT9AdymCxkWQbmKi7OZQE7r-qIFJEl9T18S6qI,54
-deep_training/nlp/layers/adalora/layers.py,sha256=0ahzA0e5kQIRhdQ_GwTSigcE1InxOtFRRbrLc39A4Zg,15143
-deep_training/nlp/layers/lora/__init__.py,sha256=An6uqZgoF7mefWEWijb3eHeZnrsqjpNA_c1KoshjjI8,72
-deep_training/nlp/layers/lora/layers.py,sha256=JWz9RtqA-hLsTxyhZPBlz82aN_VaPjNoDYRhssKV1H0,15095
-deep_training/nlp/layers/lora/utils.py,sha256=1ouFUmTF9IXzum97eIlrTeT6J4OAnEwIaWkZdgXMjSc,1819
+deep_training/nlp/layers/lora_v1/__init__.py,sha256=gmwJqLmiKqPfh5_VGWWr38y8lLgdPWw6JrjNVrvsLEY,72
+deep_training/nlp/layers/lora_v1/layers.py,sha256=JWz9RtqA-hLsTxyhZPBlz82aN_VaPjNoDYRhssKV1H0,15095
+deep_training/nlp/layers/lora_v1/utils.py,sha256=1ouFUmTF9IXzum97eIlrTeT6J4OAnEwIaWkZdgXMjSc,1819
+deep_training/nlp/layers/lora_v2/__init__.py,sha256=dGpWUx0v7UoVgwZY5srCDCBvt_hlI77zA6mQO3CxMaE,72
+deep_training/nlp/layers/lora_v2/adalora.py,sha256=y67SPRPsPPw9GjoqFKEf9v1K9WzcUGA8OOemXafqGeU,15311
+deep_training/nlp/layers/lora_v2/layers.py,sha256=SPLgtcu003bZ28gYOxPsD1rh36u16PCYDMX2yYQYdDY,8488
+deep_training/nlp/layers/lora_v2/utils.py,sha256=Hl3i9r0eP5lUzSqyPAXKnO0oEgDCY8lC3ZGV0scmNRs,9106
 deep_training/nlp/losses/BatchAllTripletLoss.py,sha256=_2Og7Hf3Bjd1GT55UFmbZq5QLxdcKUyv4T00loPrKUo,3662
 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py,sha256=Caif480bvgTWAQueadlAGSODpdaxVyRaik5-3j84wwg,3880
 deep_training/nlp/losses/BatchHardTripletLoss.py,sha256=xDdaQkcr6KCehSWlasABBkjPS9D6u_H5EngmppBkpXc,8358
 deep_training/nlp/losses/BatchSemiHardTripletLoss.py,sha256=xcfR8X3zyEs7YFoAT0q78iuZ2CJPtsrRUkp1Q8v5-QA,4552
 deep_training/nlp/losses/ContrastiveLoss.py,sha256=f7ZO4BUrqsSj0_Q670B6yIGHaSjYNOxwehBMPfRSEdg,2255
 deep_training/nlp/losses/ContrastiveTensionLoss.py,sha256=MNigl0maM6IpRasB83cf2UHPm4E73-J4N3F6y-F-uxc,4573
 deep_training/nlp/losses/CosineSimilarityLoss.py,sha256=UzWqQBE1JvASO2uZ-HzlX2YSDCLmMS-2DgoGLHqfXno,1359
@@ -89,24 +91,30 @@
 deep_training/nlp/models/w2ner.py,sha256=-KtfdpYY68s142CMcWHJbfiEHFW-qbSEENqtRgxHjBw,9025
 deep_training/nlp/models/LLaMA/__init__.py,sha256=n_M2atEv-G2i3oy_YkLCVu5QiLLyfxEj2xr91h1dWEw,16500
 deep_training/nlp/models/LLaMA/configuration.py,sha256=HNzzhIIdR9HBN9Y4Oavv6cGgIf0ExcphwsbVkltJ2ZM,5087
 deep_training/nlp/models/LLaMA_parallel/__init__.py,sha256=5lsrh09pBTzRRKwc1bJtJs37Qn5qKqif_5S0pOoD1zc,19183
 deep_training/nlp/models/LLaMA_parallel/configuration.py,sha256=HNzzhIIdR9HBN9Y4Oavv6cGgIf0ExcphwsbVkltJ2ZM,5087
 deep_training/nlp/models/PaLM/__init__.py,sha256=P1qwWPUycRmZ6I48tov6janJUNpp4L-iMoVN54ykcQw,31627
 deep_training/nlp/models/PaLM/configuration.py,sha256=kIb3nj-2pQB2wyNrYHSZqr_ta1F0Cg-VbGEbnM5icPc,5890
-deep_training/nlp/models/adalora/__init__.py,sha256=FNEb8Y0iSkO_KxDqAEShH0QAI2yEO-qA-0XT-nBOMTM,54
-deep_training/nlp/models/adalora/configuration.py,sha256=9mZ5ok08nN2-bcjblntmL4Sal3Vx9OmlpB0HaKWxVBA,54
-deep_training/nlp/models/chatglm/__init__.py,sha256=VNPZK8ySnwazfuLgcODS6vvw6coNJH9h4CuDrFeNvZg,60192
+deep_training/nlp/models/chatglm/__init__.py,sha256=VU859zidTz3HD5gT8xt2ZQr2NNU8wAnSjdY3TUz3sIk,60188
 deep_training/nlp/models/chatglm/configuration.py,sha256=4w-Kbp_FJ2crIQVyu6kie9lbMSuE3U4nnjwjVPos2E8,4575
 deep_training/nlp/models/chatglm/quantization.py,sha256=sqX_poTcYNLJLDPbCwfRllDCF0enhshjX_dw7yZa604,15150
 deep_training/nlp/models/chatglm/tokenization.py,sha256=8K8W7b2ciL8rAYlq-XEYM9p0H2NtyLn9oIUYO8zHlQo,16460
 deep_training/nlp/models/laMDA/__init__.py,sha256=fvxTQQ8jfU-msPRdC8KsGlCwzM6u8-WBmayu6gE-s0E,34123
 deep_training/nlp/models/laMDA/configuration.py,sha256=8ZvPEl1C1KUGYWw7a8XcgIgl3gWH9WXa_-ZNDqz34PE,5981
-deep_training/nlp/models/lora/__init__.py,sha256=TLkGh0MPw_-SGNP18YSnbj6SBTywqsUoiJKKt3vZb30,13316
-deep_training/nlp/models/lora/configuration.py,sha256=2CR4U2P-feBh0mwsccpLDGENSyeA0c9emu4KyAn7bqs,7058
+deep_training/nlp/models/lora/__init__.py,sha256=VoK61IC_YeFTqDhIBdhdXCqM7C3MNXc44liZkuulJBQ,44
+deep_training/nlp/models/lora/v1/__init__.py,sha256=zwGdNKqudVj7c8sMWbmZ9CnnncWXuEapAucWY-VEhLs,123
+deep_training/nlp/models/lora/v1/configuration.py,sha256=MAkg2BQCqL6XvHd2SRXsijtPToNMuN-4Hmm_02HVCmU,7054
+deep_training/nlp/models/lora/v1/lora_wrapper.py,sha256=c0mGdjE8Urop_s1i1_gLiU1igljpzVb1RUpYhJJrat4,13385
+deep_training/nlp/models/lora/v2/__init__.py,sha256=2XorjeFlyNuH6xTXiyNO1A8A3P5acBApOjxVv3YEon0,206
+deep_training/nlp/models/lora/v2/adalora_model.py,sha256=iKfKWnW--iY2gmXkMcBv6QWJr9vu-uSll57r1UNvRrY,13112
+deep_training/nlp/models/lora/v2/configuration.py,sha256=jXV4Q5yD2jkemWIHfmV7JNKT0ZEvj8rXmesjPtd53fQ,10797
+deep_training/nlp/models/lora/v2/lora_model.py,sha256=VVXH_fO5O7umaGmnp2nl4RYUrfKmkZLbQBiasKCcU1U,10398
+deep_training/nlp/models/lora/v2/lora_wrapper.py,sha256=tzDCWUiGYC81cbfNiu4ZKo3VZsftM_SF8NwH8r56BO0,10265
+deep_training/nlp/models/lora/v2/save_and_load.py,sha256=U7_ZaPm8gpg8gQhZei6UG5KvsJXDtSNZfZk1gWo6nWc,4889
 deep_training/nlp/models/splinker/__init__.py,sha256=QtgnpJa78vAq9bzfjN67NmHU3dXU6WH84jeyZoD1sBs,102
 deep_training/nlp/models/splinker/splinker.py,sha256=cAXQoPucM3ULYUhBw9z-OxPK_b9hHKEZPgMb4vFfQwc,2851
 deep_training/nlp/models/t5decoder/__init__.py,sha256=R9Op4Ysli9isootQQ2FcjhpbG13fNESlmUROu6cfGH0,14478
 deep_training/nlp/models/t5encoder/__init__.py,sha256=692ChfLf2sZWgzhBM37g1PdpmEmsU1R9RRl_uTHRET0,6646
 deep_training/nlp/optimizer/__init__.py,sha256=c4cmx9ebIdqwXBu3N9QbcNNHb32t2MV6fTK9aC2VBGQ,56
 deep_training/nlp/optimizer/lamb.py,sha256=htvZQHPWHG5GCDgo9xCaZikWwRyaD2PjDioIQvX7qXw,5225
 deep_training/nlp/optimizer/lion/__init__.py,sha256=AvYkLp7sOpRIC3a5ejuniUUKyQmmBA1TPJdt2RA7Nqg,99
@@ -126,11 +134,11 @@
 deep_training/tfnlp/scheduler/__init__.py,sha256=69flKnae4cQQyWUDwuYE0w0iaPonvH0P_WjBd_t-IqU,53
 deep_training/tfnlp/utils/__init__.py,sha256=kAmlOWNSpQCHbtT-mAsKGQzQFoWKp2jQf3neCJ0cCRY,53
 deep_training/utils/__init__.py,sha256=JFm7m_LPsS9Oavyxn9rbWqllCmV_zBho19rISlHNX4c,55
 deep_training/utils/distributed.py,sha256=-dhvJ6YHpRxvtZ1_on50IE33fUFW3zKXBKqqK-L1HGM,1941
 deep_training/utils/func.py,sha256=1p8hiQDCyk_gQGKrF7y6Dt66k3jLXSAt2IQeJuHQEl8,1724
 deep_training/utils/maskedlm.py,sha256=o8EB2BbDdh7wdgqz9Oi6SsVr1uBWxV15qfTk2VPjWsU,5117
 deep_training/utils/trainer.py,sha256=Rit5xEC2r9MvQdDR4A5A6E4_gzNCVNmW9m55kC83O50,7469
-deep_training-0.1.1.dist-info/METADATA,sha256=TvHlY35shbp2hzAbzR6y3Qzsl0a1A-pAZ3mMvaH8fq4,603
-deep_training-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-deep_training-0.1.1.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
-deep_training-0.1.1.dist-info/RECORD,,
+deep_training-0.1.2rc0.dist-info/METADATA,sha256=nffasjbmMO06ENSfOG0rzsQw-SUBA2IZ9pCBI_cJPRY,626
+deep_training-0.1.2rc0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+deep_training-0.1.2rc0.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
+deep_training-0.1.2rc0.dist-info/RECORD,,
```

