# Unix - Generic stuff

## Change line endings

### Via Vim
```
:set ff=unix
```

## Remove ansi codes
```
sed -r "s/\x1b\[([0-9]{1,2}(;[0-9]{1,2})?)?m//g" < ansi.log > noansi.log
```

## Check pfx
```
openssl pkcs12 -in signing.pfx -nokeys | openssl x509 -text -noout
```
