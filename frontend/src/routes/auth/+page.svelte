<script>
    import Navbar from "$lib/navbar.svelte";
    import Footer from "$lib/footer.svelte";
</script>

<Navbar />

<div class="flex justify-center-safe gap-3">
    <a href="/auth/login" class=" font-extrabold"> Login </a>
    <a href="auth/register" class=" font-extrabold"> Registrati </a>
</div>
<div>
    <p class="flex justify-center">
        Welcome to C-Trends, ready to enter the reality?
    </p>
</div>
<Footer />
