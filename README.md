1. Here model is getting serve via tensorflow serving , which is a open source serving 
2. convert your model into tf serving saved model format(ref: "https://docs.ultralytics.com/integrations/tf-savedmodel/#usage")
3. once your model has been converted in saved model format put that into detection_tfv/models folder
4. In dockerfile line number 35 chnage the model name and path according to your model name and path.
5. This is cpu based , so 1st try with a small video in cpu else you can just pass the GPU allocation parameters into it.
6. If using GPU please pass the GPU parameter in docker compose
7. Change the port as per your requirement.
