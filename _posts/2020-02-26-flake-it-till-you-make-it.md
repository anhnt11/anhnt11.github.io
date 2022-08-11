---
layout: post
title: Flake it till you make it
subtitle: Excerpt from Soulshaping by Jeff Brown
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/thumb.png
share-img: /assets/img/path.jpg
tags: [books, test]
---

<html xmlns:th="http://www.thymeleaf.org">
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Create student</title>
</head>
<body>
<!--Các bạn có thể tìm hiểu thêm  phần này tại blogs: https://levunguyen.com,-->
<!--blogs chuyên về lập trình và các kỹ năng mềm trong nghề lập trình-->
    <form th:action="@{/create}" th:method="post" th:object="${student}">
        <label>Name: </label>
        <input type="text" th:field="*{name}"/><br>
        <label>Date of birth: </label>
        <input type="text" th:field="*{dateOfBirth}"/><br>
        <input type="submit" value="Register" />
    </form>
</body>
</html>
