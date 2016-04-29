This is a MD4 algorithm function wrote in powershell.

PS> Get-MD4 -String 'abc' -UpperCase
A448017AAF21D8525FC10AE87AA6729D

PS> $b = @('abc'.ToCharArray() | %{[int]$_})
PS> Get-MD4 -bArray $b
a448017aaf21d8525fc10ae87aa6729d

Reference: https://tools.ietf.org/html/rfc1320
MD4 algorithm is old and replaced by MD5 and many others due to security defects
MD4 algorithm is still the one-way-function encryption algorithm for Windows NT passwords.

 - Larry.Song@outlook.com