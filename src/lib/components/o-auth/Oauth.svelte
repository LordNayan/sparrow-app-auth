<script>
    import googleLogo from '$lib/assets/googlelogo.svg';
	import constants from '$lib/utils/constants';
	import { navigate } from 'svelte-navigator';
    const handleSignInWithGoogle = async () => {
		navigate(constants.SPARROW_OAUTH);
	};
</script>
<div class="d-flex flex-column align-items-center justify-content-center">
    <p>or continue with</p>
    <div class="d-flex gap-4">
        <button
            on:click={handleSignInWithGoogle}
            style="width: 32px; height:32px"
            class="bg-backgroundDark border-0 rounded"
        >
            <img src={googleLogo} alt="Google Logo" class="w-100 h-100 p-1" />
        </button>
    </div>
</div>