Project Overview


In this project, I explored various methods for measuring similarity between documents and images. The primary focus was on implementing and combining different similarity metrics to enhance the accuracy of matching documents and images.
Approach and Files

If you want to have a look at the particular files and results of different approaches, you can refer to this "https://github.com/yourselfthere/docSimilarpy.git".

1. Cosine Similarity

Initially, I approached the problem by implementing the Cosine Similarity metric. This metric measures the cosine of the angle between two vectors in a multi-dimensional space, which helps determine the orientation of the vectors.

    File: cosine.ipynb
    Description: This notebook demonstrates the application of the Cosine Similarity metric for comparing document features.
    Results: The results and analysis of using Cosine Similarity can be found in this file.

2. Jaccard Similarity

Following the exploration of Cosine Similarity, I implemented the Jaccard Similarity metric. This metric measures the similarity between two sets by dividing the size of their intersection by the size of their union.

    File: cosineJaccard.ipynb
    Description: This notebook shows the combination of Cosine Similarity and Jaccard Similarity metrics for feature extraction and comparison.
    Results: The results and comparisons can be found in this file.

3. Structural Similarity Index (SSIM)

Next, I investigated the Structural Similarity Index (SSIM), which assesses the similarity between two images by considering luminance, contrast, and structure.

    File: SSIM.ipynb
    Description: This notebook details the use of SSIM for image similarity measurement.
    Results: The results of using SSIM are documented in this file.

4. Feature Extraction with VGG16

After researching further, I decided to use the VGG16 model for feature extraction. VGG16 is a convolutional neural network model that is pre-trained on the ImageNet dataset. It is known for its deep architecture and ability to extract detailed features from images.
So first i converted the documents from pdf to jpg.
    File: VGG16.ipynb
    Description: This notebook explains how VGG16 is used for feature extraction and its integration with similarity metrics.
    Results: Combining VGG16 features with SSIM showed improved results.

5. Combining Metrics

To leverage the strengths of different metrics, I combined VGG16 feature extraction with Cosine Similarity and SSIM. This approach aimed to incorporate the best aspects of each metric.

    File: VGG16cosSSIM.ipynb
    Description: This notebook explores the combination of VGG16 and SSIM metrics for enhanced similarity measurement.
    Results: The results showed significant improvement in similarity assessment.

6. Final Approach- and the best results

The final approach combined Cosine Similarity, VGG16 feature extraction, and Jaccard Similarity. This combination aimed to utilize Cosine Similarity for orientation, VGG16 for detailed feature extraction, and Jaccard Similarity for entity matching.

    File: VGG16cosJac.ipynb
    Description: This notebook details the integration of Cosine Similarity, VGG16, and Jaccard Similarity metrics.
    Results: The best results were achieved with this approach, providing a comprehensive similarity measure.

RESULTS : 
Test Image: invoice_77098.jpg
Most Similar Image: invoice_77073.jpg
Similarity Score: 0.9861023215324117


Test Image: invoice_102857.jpg
Most Similar Image: invoice_102856.jpg
Similarity Score: 0.9614406268093565



Conclusion

The combination of VGG16 feature extraction with Cosine Similarity and Jaccard Similarity provided the best results for document and image similarity. This approach effectively incorporates the strengths of different similarity metrics for improved accuracy.


