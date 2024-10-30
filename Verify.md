# Verify
So open the files in the webshell after launching the instance, since we have a checkSum file and a decrypt hash file we can assume that we need to do a sha256 sum of the load of files we have, i realized that after the hint tbh.

So, execute `sha256sum files/*` and you will get all the sums, now pipe grep with checksum to get the required file.

Then run the decrypt file, `./decrypt files/451fd69b`.

Flag: picoCTF{trust_but_verify_451fd69b}
