<script>
    let email = "";
    let password = "";

    function handleSubmit() {
        // Qui puoi gestire il login (API, validazione, ecc.)
        console.log("Email:", email, "Password:", password);
    }
</script>

<div class="flex flex-col items-center justify-center min-h-screen bg-gray-50">
    <form
        class="w-full max-w-md space-y-6 bg-white p-8 rounded-lg shadow"
        on:submit|preventDefault={handleSubmit}
    >
        <h1 class="text-2xl font-bold text-center mb-6">Login</h1>

        <!-- Campo Email -->
        <div class="flex flex-col gap-2">
            <label for="email" class="text-sm font-medium">Email</label>
            <input
                type="email"
                id="email"
                bind:value={email}
                placeholder="Inserisci la tua email"
                required
                class="px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
        </div>

        <!-- Campo Password -->
        <div class="flex flex-col gap-2">
            <label for="password" class="text-sm font-medium">Password</label>
            <input
                type="password"
                id="password"
                bind:value={password}
                placeholder="Inserisci la tua password"
                required
                class="px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500"
            />
        </div>

        <!-- Bottone Login -->
        <button
            type="submit"
            class="w-full bg-blue-500 text-white py-2 px-4 rounded-lg font-bold hover:bg-blue-600"
        >
            Accedi
        </button>
    </form>
</div>
