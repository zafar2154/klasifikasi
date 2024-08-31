# klasifikasi

docker run -it --rm -v C:\python\ML\klasifikasi:/klasifikasi -p 8501:8501 --entrypoint /bin/bash tensorflow/serving

tensorflow_model_server --rest_api_port=8501 --model_name=classify --model_base_path=/klasifikasi/klasifikasi_model

http://localhost:8501/v1/models/classify

{
  "model_version_status": [
    {
      "version": "1",
      "state": "AVAILABLE",
      "status": {
        "error_code": "OK",
        "error_message": ""
      }
    }
  ]
}


