---
title: About
icon: fas fa-info
order: 4
---
<style>
    .pie_wrapper{
        display : flex;
        justify-content:center;
        align-items:center;
    }
    .rank{
        width : 500px;
        padding-left : 20px
    }
    .solve-wrapper{
        display: flex;
    }
    .solve-wrapper > div{
        display: flex;
    }
    .pie_chart{
        width: 300px;
        height: 300px;
        background-image : url('/images/pie.png');
        background-position : center;
        background-size : cover;
    }
    .solve{
        display: flex;
        flex-direction: column;
        justify-content: end;
    }
    .solve-table > tbody > tr > td{
        text-align: end;
    }
    .bronze > th{
        color : #ad5600;
    }
    .silver > th{
        color : #435f7a;
    }
    .gold > th{
        color : #ec9a00;
    }
    .platinum > th{
        color : #27e2a4;
    }
    .diamond > th{
        color : #00b4fc;
    }
    .ruby > th{
        color : #ff0062;
    }
    .profile_wrapper{
        display: flex;
        align-items: center;

    }
    .profile_picture{
        background-image: url('/images/profile.jpeg');
        height : 200px;
        width : 200px;
        background-size : cover;
        background-position : center;
        border-radius : 30%;
    }
</style>
<div class="profile_wrapper">
    <div class="proflie_picture_wrapper">
        <div class="profile_picture">
        </div>
    </div>
    <div style="margin-left : 30px">
        <ul class="list-group list-group-flush">
            <h2>김덕휘</h2>
            <li class="list-group-item">-1996년 출생</li>
            <li class="list-group-item">-2018년 ROKMC 전역</li>
            <li class="list-group-item">-2021년 연세대학교 컴퓨터과학과 졸업</li>
        </ul>      
    </div>
</div>
<h2 style = "font-weight: bold">
    Solved.ac
    <span style="text-align: end;">
        <img src="/images/tier.svg" height="40px" >
    </span>
</h2>
<div class="solve-wrapper" >
    <div class="pie_wrapper">
        <div class="pie_chart">
        </div>
    </div>
    <div class="rank" >
        <table class="table solve-table">
            <thead>
                <tr>
                <th scope="col">레벨</th>
                <th scope="col" style="text-align: end;">문제</th>
                <th scope="col" style="text-align: end;">경험치</th>
                </tr>
            </thead>
            <tbody>
                <tr class="bronze">
                <th scope="row">BRONZE</th>
                <td>59</td>
                <td>54,528</td>
                </tr>
                <tr class ="silver">
                <th scope="row">SILVER</th>
                <td>101</td>
                <td>854,567</td>
                </tr>
                <tr class ="gold">
                <th scope="row">GOLD</th>
                <td>167</td>
                <td>9,669,027</td>
                </tr>
                <tr class ="platinum">
                <th scope="row">PLATINUM</th>
                <td>35</td>
                <td>8,290,013</td>
                </tr>
                <tr class ="diamond">
                <th scope="row">DIAMOND</th>
                <td>0</td>
                <td>0</td>
                </tr>
                <tr class ="ruby">
                <th scope="row">RUBY</th>
                <td>0</td>
                <td>0</td>
                </tr>
            </tbody>
        </table>
    </div>
</div>

# 개발 로그

# Ebbeum 
***
[Repository Link](https://github.com/TheKeyKim/Ebbeum)

> 프레임워크 : react-native

> 파트 : FE

이븜은 리액트 네이티브 프레임워크를 기반으로한 android, ios 어플리케이션입니다. 회원, 비회원 이용을 지원하며, 체형 입력을 통해 각자의 체형에 어울릴만한 스타일의 옷을 추천해주는 어플리케이션입니다. 

<p align="center">
<image src="/images/Ebbeum_0.png" height="300px" />
<image src="/images/Ebbeum_1.jpeg" height="300px" />
<image src="/images/Ebbeum_2.jpeg" height="300px" />
<image src="/images/Ebbeum_3.png" height="300px" />
</p>
***
<br>

# The Keys Judge - FE
***
[Repository Link](https://github.com/TheKeyKim/thekeysjudge) <br>
[Page Link](https://thekeykim.github.io/thekeysjudge/)
> 프레임 워크 : vue.js vuex 

> 파트 : FE

백준 온라인 저지의 클론 사이트이며, 학습을 목적으로 제작되었습니다. 대부분의 asset은 BOJ사이트의 것을 사용하였습니다.

<p align="center">
<image src="/images/TOJ_0.png" />
</p>
***
<br>

# The Keys Judge - BE
***
[Repository Link](https://github.com/TheKeyKim/TOJ-server)

> 프레임 워크 : Node.js Mysql Sequelize

> 파트 : BE

Thekeys judge 백준 클론 사이트를 위한 서버입니다. 로그인과 회원가입, 문제의 정보 가져오기 및 채점 서버를 포함합니다. 다음의 api를 제공합니다.

1. 회원가입
2. 로그인
3. 문제 정보 가져오기
4. C++, Java, Python 언어에 대한 채점(미완성)

채점에 대한 로직은 shell script 및 문제적 허용 체크, 아웃풋 무결성 체크를 위한 C++ 어플리케이션을 이용하여 구동됩니다.

## submit
- post
- problem/submit
- login is needed
```
{
    "id" : Number,
    "problem_id" : Number,
    "language" : Number,
    "code" : String
}
```
(사용예시)
```json
{
    "id" : 1,
    "problem_id" : 1000,
    "language" : 0,
    "code" : "#include<iostream>\nusing namespace std;\nint main(void){\n int a, b;\n cin>>a>>b;\ncout<<a+b<<endl;}\n"
}
```












