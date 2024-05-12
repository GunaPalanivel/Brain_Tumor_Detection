# Brain Tumor Detection

Brain tumor is an abnormal growth of cells within the brain or surrounding tissues, categorized as either benign or malignant. They can originate in the brain or spread from elsewhere in the body. Symptoms vary but may include headaches, seizures, vision changes, and personality shifts. Diagnosis involves medical history assessment, physical exams, imaging, and sometimes biopsies. Treatment options depend on tumor type and may include surgery, radiation, chemotherapy, targeted therapy, or immunotherapy. Prognosis varies, with early diagnosis and tailored treatment improving outcomes. Follow-up care and monitoring are often necessary after treatment to manage potential recurrences or side effects.

## Requirements

opencv

pillow

tensorflow

## Tumor Detection
The GUI can be used to detect and view the tumor region.

The tensorflow model can be used to detect if the MRI image contains tumor or not.

![alt text](tumordetection.jpg)

The tumor region can be viewed using Image processing methods applied through opencv. Image segmentation using marker-based watershed segmentation algorithm is used to view the tumor region. A watershed is a transformation defined on a grayscale image. We label the region which we are sure of being the foreground or object with one color(or intensity), and label the region which we are sure of being background or non-object with another color and finally the region which we are not sure of anything, we label it with 0. That is our marker. Then apply watershed algorithm. Then our marker will be updated with the labels we gave, and the boundaries of objects will have a value of -1.

![alt text](viewtumor.jpg)
