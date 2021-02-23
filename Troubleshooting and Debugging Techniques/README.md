# Troubleshooting and Debugging Techniques

![Certification](https://user-images.githubusercontent.com/41291493/108625432-4531c600-748e-11eb-9e76-82644ace4591.png)

## Learning Objectives
* What is debugging
* Binary Searching a Problem
* Finding Invalid Data
* Looking into what causes slow scripts, slow computers, or slow systems
* Looking into what tools are there to help identify the most common causes of slowness, and apply solutions to improve the overall performance
* Why Programs Crash
* What to do when you can't fix the program
* Understand to Internal Server Error
* Accessing Invalid Memory
* Debugging a Segmentation Fault
* Handling Bigger Incidents
* Managing Computer Resources
* Managing Our Time

### Note

```
파이썬 코드를 통한 자원 확인
> psutil.cpu_percent()
> psutil.disk_io_counters()
> psutil.net_io_counters()

코어 파일 활성화
$ ulimit -c unlimited

gbg 디버거를 통한 Segmentation Fault 분석
$ gbg -c core example(file)

충돌이 난 로그를 추적하는 명령어
$ backtrace 

보편적으로 gdb는 C, C++ 기반의 바이너리에 사용하고, python 코드는 pdb3를 사용한다.

파이썬 디버거를 통한 파이썬 코드 디버깅
$ pdb3 test.py {parameter}

```

---
