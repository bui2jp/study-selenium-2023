# study-selenium-2023

![img](./selenium-chrome.drawio.png)

## docker image

```
docker pull selenium/standalone-chrome
```

## docker run

```
docker run --rm -d -p 4444:4444 -p 7900:7900 --dns=8.8.8.8 --shm-size="2g" selenium/standalone-chrome:latest
```

## pythonからseleniumを使う

run
```
docker pull python
#docker run -it --rm -w /home -v $(pwd):/home --dns=8.8.8.8 python bash
docker run -it --rm -w /home -v $(pwd):/home --dns=8.8.8.8 python python ./t001.py
```

run via Dockerfile
```
docker build -t my-python-test .
docker run -it --rm my-python-test
```

## Selenium IDE (chrome extention) 
pythonのコードを生成することもできる


