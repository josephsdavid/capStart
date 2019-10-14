
# Deep learning of joint myelin and T1w MRI features in normal-appearing brain tissue to distinguish between multiple sclerosis patients and healthy controls

source : **<https://doi.org/10.1016/j.nicl.2017.10.015>**

In summary, our experimental results have demonstrated the following for the
task of detecting MS pathology on normal-appearing brain tissues:

* The regional mean myelin content features were more discriminative than the
regional mean T1w intensity features.

* Direct concatenation of the regional mean myelin content features and the
regional mean T1w intensity features did not improve the classification accuracy
over using each feature type alone.

* Unsupervised deep learning of the regional myelin contents and T1w intensities
yielded superior classification performance over using the regional mean myelin
contents and T1w intensities.

* The joint deep-learned regional myelin-T1w features were more discriminative
than either of the modality-specific deep-learned feature types.

* Applying LASSO to produce sparser feature representations improved the
classification performance for the regional mean features, but the impact of
LASSO was marginal for the deep-learned regional features.

* The maximum classification performance of using predominantly NAWM and NAGM
patches separately was achieved by the deep-learned regional myelin features.
However, it did not approach that of using all normal-appearing patches
together.
