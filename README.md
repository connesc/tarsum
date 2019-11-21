# tarsum

Compute checksums from tar archives on-the-fly.

```
Usage: tarsum md5|sha1|sha224|sha256|sha384|sha512|b2 [TAR OPTIONS...]
```

## Examples

```sh
tarsum b2 < archive.tar > checksums.b2
```

```sh
tarsum sha256 -f archive.tar | diff checksums.sha256 -
```

```sh
zcat archive.tar.gz | tarsum sha1 > checksums.sha1
```

```sh
curl https://example.com/archive.tar.xz | tarsum md5 -J > checksums.md5
```

## License

[ISC License](LICENSE)

