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
                <td>58</td>
                <td>52,526</td>
                </tr>
                <tr class ="silver">
                <th scope="row">SILVER</th>
                <td>76</td>
                <td>631,018</td>
                </tr>
                <tr class ="gold">
                <th scope="row">GOLD</th>
                <td>118</td>
                <td>6,465,112</td>
                </tr>
                <tr class ="platinum">
                <th scope="row">PLATINUM</th>
                <td>22</td>
                <td>4,968,421</td>
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

