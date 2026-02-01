UNET -
A medical image segmentation project using UNet to identify and segment skin lesions/allergies from dermoscopic images. This implementation focuses on robust segmentation through combined loss functions.


Problem: Segmenting skin lesions/allergies from dermoscopic images for potential medical analysis. This serves as medical image segmentation practice with real clinical relevance.

 **Exploding Loss** -> During training, the model faced exploding gradients/loss, making convergence difficult.
solution was combined loss ->
                      **DICE-LOSS** -> dice loss help us by penalizing the non overlapping area which we want to overlap , which is subtle in segmntation 
                      **FOCAL-LOSS** -> focal loss help us by forcing the model to loopup on the hard cases like border ones too. that's why it help in heavy penalizing when model try to learns explicitly.

**why UNET??**
 While architectures like ResNet exist, UNet's skip connections are ideal for medical imaging because:

        Preserves spatial information crucial for lesion localization
        
        Handles varying lesion sizes (small spots to large patches)
        
        Maintains fine details at lesion boundaries
        
        Proven track record in medical imaging competitions (ISIC challenges)


https://drive.google.com/file/d/193NpUaiwWkcWHJ-QjsDbLQrxaiX1yXZw/view?usp=drive_link 


use this link for weigths
