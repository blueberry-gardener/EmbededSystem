<style>
body {
    counter-reset: h1;
}
h1 {
    counter-reset: h2;
}
h2 {
    counter-reset: h3;
}
h1:before {
    counter-increment: h1+2;
    content: counter(h1) ". ";
}
h2:before {
    counter-increment: h2;
    content: counter(h1) "." counter(h2) ". ";
}
h3:before {
    counter-increment: h3;
    content: counter(h1) "." counter(h2) "."counter(h3) ". ";
}
</style>

# CPU

## 



***
[TopPage](./README.md)