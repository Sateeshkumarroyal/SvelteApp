<script>
import {goto, beforeNavigate, afterNavigate} from '$app/navigation';
const handleclick = () => {
    goto('/products);
};

beforeNavigate((navigate) => {
    console.log({ before:navigation});
});

afterNavigateNavigate((navigate) => {
    console.log({ after:navigation});
});
</script>
<h1>Welcome Home</h1>
<a href="/blog">Blog</a>
<a href="/products">Products</a>
<a href="/about">About</a>
<a href="/profile">Profile</a>

<button on:click={handleclick}>Submitt</button>
