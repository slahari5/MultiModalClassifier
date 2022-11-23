# Options Selected:
* Inference using OpenVino
* Serving with Rest API

Datasets Used:
* For OpenVino :
https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz
* For RestAPIs:


Colab:
https://colab.research.google.com/drive/160AD-r_ylPugdn01Zi2aDrpulTuIWKPC?usp=sharing

Github link:

# 1. Inference using OpenVino 

model_name = "flower"
model_path = Path(model_fname)
ir_data_type = "FP16"
ir_model_name = "flower_ir"


Command for Model Optimizer:
mo_command = f"""mo
                 --saved_model_dir "{model_fname}"
                 --input_shape "[1,180,180,3]"
                 --data_type "{ir_data_type}"
                 --output_dir "{model_fname}"
                 --model_name "{ir_model_name}"
                 """
mo_command = " ".join(mo_command.split())

Steps :
Downloaded the dataset of flowers which has 5 differenct species consisting of 3670 samples.

Tensorflow framework has been used to train the dataset.

Loaded the dataset 

Trained the model on google colab using the python script 

Trained the model for 25 epochs
![image](https://user-images.githubusercontent.com/99698941/203488042-4fc9ac5c-989f-4783-92f6-c09fe7af4b51.png)


Took the inference for val dataset. 
Got good prediction on val data with a confidence of 99.
![image](https://user-images.githubusercontent.com/99698941/203488186-6b4e0342-b895-4c41-b6f6-d569b2142084.png)

