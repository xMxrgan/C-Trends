<script>
    let mail = "";
    let password = "";

    async function handleSubmit() {
        console.log("E-mail: ", mail, "Password ", password);

        if (mail.includes("@")) {
            let error = "Mail non valida!";
            return;
        }

        if (password.length <= 6) {
        }
    }
</script>

<div>
    <p>Login</p>
    <label for="E-mail">Mail</label>
</div>

<div>
    <label for="E-mail">Password</label>
</div>
