# 3rd Project TEAM 2

## STREAMLIT 
### Usage
- 전제 조건 : DB와 FastAPI가 동일한 Docker 환경 내에 실행되고 있어야 함
```bash
# Run Streamlit
$ sudo docker run -d -p 8032:8501 -e EC2_IP=<docker_ip> -e PWD=<admin_pwd> -v /home/ubuntu/images:/home/ubuntu/images --name stream j25ng/streamlit:8.0.0
```
```
# Streamlit page URL 예시
http://<your_ip>:8032
```

### 기능
#### User Page
- Upload Image
![image](https://github.com/user-attachments/assets/c6961226-c6c5-4ca5-8218-4790e477e25f)
- View Result
![image](https://github.com/user-attachments/assets/b5a0f868-a6a9-4f84-8de3-c0ecefbc99e4)
- View Chart
![image](https://github.com/user-attachments/assets/032523cd-0578-4483-bb84-02c4e91b3660)
![image](https://github.com/user-attachments/assets/d13f10e0-5c9b-477f-aeed-300609a86443)
![image](https://github.com/user-attachments/assets/5e154209-502c-452f-8d32-d14e51c5fca9)

#### Admin Page
- Input Password : <admin_pwd>로 로그인
![image](https://github.com/user-attachments/assets/f04d9918-3d62-4cab-bac2-615ca6e23760)
- Dashboard
![image](https://github.com/user-attachments/assets/7d8f6b93-68e8-4684-a7eb-350171f08b5f)

