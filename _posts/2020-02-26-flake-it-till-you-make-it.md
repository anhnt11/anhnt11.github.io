

<html xmlns:th="http://www.thymeleaf.org">
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    **Create student**
</head>
<body>
    <form th:action="@{/create}" th:method="post" th:object="${student}">
        <label>Name: </label>
        <input type="text" th:field="*{name}"/><br>
        <label>Date of birth: </label>
        <input type="text" th:field="*{dateOfBirth}"/><br>
        <input type="submit" value="Register" />
    </form>
</body>
</html>
