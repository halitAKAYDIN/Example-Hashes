<div class="page">

</div>
</div>
<!-- TOC END -->

<h1 class="sectionedit1" id="example_hashes">Example hashes</h1>
<div class="level1">

<p>
If you get a “line length exception” error in hashcat, it is often because the hash mode that you have requested does not match the hash. To verify, you can test your commands against example hashes.
</p>

<p>
Unless otherwise noted, the password for all example hashes is <strong>hashcat</strong>.
</p>

</div>

<h1 class="sectionedit2" id="generic_hash_types">Generic hash types</h1>
<div class="level1">
<div class="plugin_tablelayout_placeholder" data-tablelayout="{&quot;colwidth&quot;:[&quot;60px&quot;,&quot;340px&quot;,&quot;540px&quot;],&quot;rowsHeaderSource&quot;:&quot;1&quot;,&quot;rowsVisible&quot;:&quot;0&quot;,&quot;float&quot;:&quot;left&quot;}"></div><div class="table sectionedit3"><table class="inline">
	<thead>
	<tr class="row0">
		<th class="col0"> Hash-Mode </th><th class="col1"> Hash-Name </th><th class="col2"> Example </th>
	</tr>
	</thead>
	<tbody><tr class="row1">
		<td class="col0"> 0 </td><td class="col1"> MD5 </td><td class="col2"> 8743b52063cd84097a65d1633f5c74f5 </td>
	</tr>
	<tr class="row2">
		<td class="col0"> 10 </td><td class="col1"> md5($pass.$salt) </td><td class="col2"> 01dfae6e5d4d90d9892622325959afbe:7050461 </td>
	</tr>
	<tr class="row3">
		<td class="col0"> 20 </td><td class="col1"> md5($salt.$pass) </td><td class="col2"> f0fda58630310a6dd91a7d8f0a4ceda2:4225637426 </td>
	</tr>
	<tr class="row4">
		<td class="col0"> 30 </td><td class="col1"> md5(utf16le($pass).$salt) </td><td class="col2"> b31d032cfdcf47a399990a71e43c5d2a:144816 </td>
	</tr>
	<tr class="row5">
		<td class="col0"> 40 </td><td class="col1"> md5($salt.utf16le($pass)) </td><td class="col2"> d63d0e21fdc05f618d55ef306c54af82:13288442151473 </td>
	</tr>
	<tr class="row6">
		<td class="col0"> 50 </td><td class="col1"> HMAC-MD5 (key = $pass) </td><td class="col2"> fc741db0a2968c39d9c2a5cc75b05370:1234 </td>
	</tr>
	<tr class="row7">
		<td class="col0"> 60 </td><td class="col1"> HMAC-MD5 (key = $salt) </td><td class="col2"> bfd280436f45fa38eaacac3b00518f29:1234 </td>
	</tr>
	<tr class="row8">
		<td class="col0"> 100 </td><td class="col1"> SHA1 </td><td class="col2"> b89eaac7e61417341b710b727768294d0e6a277b </td>
	</tr>
	<tr class="row9">
		<td class="col0"> 110 </td><td class="col1"> sha1($pass.$salt) </td><td class="col2"> 2fc5a684737ce1bf7b3b239df432416e0dd07357:2014 </td>
	</tr>
	<tr class="row10">
		<td class="col0"> 120 </td><td class="col1"> sha1($salt.$pass) </td><td class="col2"> cac35ec206d868b7d7cb0b55f31d9425b075082b:5363620024 </td>
	</tr>
	<tr class="row11">
		<td class="col0"> 130 </td><td class="col1"> sha1(utf16le($pass).$salt) </td><td class="col2"> c57f6ac1b71f45a07dbd91a59fa47c23abcd87c2:631225 </td>
	</tr>
	<tr class="row12">
		<td class="col0"> 140 </td><td class="col1"> sha1($salt.utf16le($pass)) </td><td class="col2"> 5db61e4cd8776c7969cfd62456da639a4c87683a:8763434884872 </td>
	</tr>
	<tr class="row13">
		<td class="col0"> 150 </td><td class="col1"> HMAC-SHA1 (key = $pass) </td><td class="col2"> c898896f3f70f61bc3fb19bef222aa860e5ea717:1234 </td>
	</tr>
	<tr class="row14">
		<td class="col0"> 160 </td><td class="col1"> HMAC-SHA1 (key = $salt) </td><td class="col2"> d89c92b4400b15c39e462a8caa939ab40c3aeeea:1234 </td>
	</tr>
	<tr class="row15">
		<td class="col0"> 200 </td><td class="col1"> MySQL323 </td><td class="col2"> 7196759210defdc0 </td>
	</tr>
	<tr class="row16">
		<td class="col0"> 300 </td><td class="col1"> MySQL4.1/MySQL5 </td><td class="col2"> fcf7c1b8749cf99d88e5f34271d636178fb5d130 </td>
	</tr>
	<tr class="row17">
		<td class="col0"> 400 </td><td class="col1"> phpass, WordPress (MD5),<br>
Joomla (MD5) </td><td class="col2"> $P$984478476IagS59wHZvyQMArzfx58u. </td>
	</tr>
	<tr class="row18">
		<td class="col0"> 400 </td><td class="col1"> phpass, phpBB3 (MD5) </td><td class="col2"> $H$984478476IagS59wHZvyQMArzfx58u. </td>
	</tr>
	<tr class="row19">
		<td class="col0"> 500 </td><td class="col1"> md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) <sup>2</sup> </td><td class="col2"> $1$28772684$iEwNOgGugqO9.bIz5sk8k/ </td>
	</tr>
	<tr class="row20">
		<td class="col0"> 501 </td><td class="col1"> Juniper IVE </td><td class="col2 leftalign"> 3u+UR6n8AgABAAAAHxxdXKmiOmUoqKnZlf8lTOhlPYy93EAkbPfs5+49YLFd/B1+omSKbW7DoqNM40/EeVnwJ8kYoXv9zy9D5C5m5A==  </td>
	</tr>
	<tr class="row21">
		<td class="col0"> 600 </td><td class="col1"> BLAKE2b-512 </td><td class="col2"> $BLAKE2$296c269e70ac5f0095e6fb47693480f0f7b97ccd0307f5c3bfa4df8f5ca5c9308a0e7108e80a0a9c0ebb715e8b7109b072046c6cd5e155b4cfd2f27216283b1e </td>
	</tr>
	<tr class="row22">
		<td class="col0"> 900 </td><td class="col1"> MD4 </td><td class="col2"> afe04867ec7a3845145579a95f72eca7 </td>
	</tr>
	<tr class="row23">
		<td class="col0"> 1000 </td><td class="col1"> NTLM </td><td class="col2"> b4b9b02e6f09a9bd760f388b67351e2b </td>
	</tr>
	<tr class="row24">
		<td class="col0"> 1100 </td><td class="col1"> Domain Cached Credentials (DCC), MS Cache </td><td class="col2"> 4dd8965d1d476fa0d026722989a6b772:3060147285011 </td>
	</tr>
	<tr class="row25">
		<td class="col0"> 1300 </td><td class="col1"> SHA-224 </td><td class="col2"> e4fa1555ad877bf0ec455483371867200eee89550a93eff2f95a6198 </td>
	</tr>
	<tr class="row26">
		<td class="col0"> 1400 </td><td class="col1"> SHA-256 </td><td class="col2"> 127e6fbfe24a750e72930c220a8e138275656b8e5d8f48a98c3c92df2caba935 </td>
	</tr>
	<tr class="row27">
		<td class="col0"> 1410 </td><td class="col1"> sha256($pass.$salt) </td><td class="col2"> c73d08de890479518ed60cf670d17faa26a4a71f995c1dcc978165399401a6c4:53743528 </td>
	</tr>
	<tr class="row28">
		<td class="col0"> 1420 </td><td class="col1"> sha256($salt.$pass) </td><td class="col2"> eb368a2dfd38b405f014118c7d9747fcc97f4f0ee75c05963cd9da6ee65ef498:560407001617 </td>
	</tr>
	<tr class="row29">
		<td class="col0"> 1430 </td><td class="col1"> sha256(utf16le($pass).$salt) </td><td class="col2"> 4cc8eb60476c33edac52b5a7548c2c50ef0f9e31ce656c6f4b213f901bc87421:890128 </td>
	</tr>
	<tr class="row30">
		<td class="col0"> 1440 </td><td class="col1"> sha256($salt.utf16le($pass)) </td><td class="col2"> a4bd99e1e0aba51814e81388badb23ecc560312c4324b2018ea76393ea1caca9:12345678 </td>
	</tr>
	<tr class="row31">
		<td class="col0"> 1450 </td><td class="col1"> HMAC-SHA256 (key = $pass) </td><td class="col2"> abaf88d66bf2334a4a8b207cc61a96fb46c3e38e882e6f6f886742f688b8588c:1234 </td>
	</tr>
	<tr class="row32">
		<td class="col0"> 1460 </td><td class="col1"> HMAC-SHA256 (key = $salt) </td><td class="col2"> 8efbef4cec28f228fa948daaf4893ac3638fbae81358ff9020be1d7a9a509fc6:1234 </td>
	</tr>
	<tr class="row33">
		<td class="col0"> 1500 </td><td class="col1"> descrypt, DES (Unix), Traditional DES </td><td class="col2"> 48c/R8JAv757A </td>
	</tr>
	<tr class="row34">
		<td class="col0"> 1600 </td><td class="col1"> Apache $apr1$ MD5, md5apr1, MD5 (APR) <sup>2</sup> </td><td class="col2"> $apr1$71850310$gh9m4xcAn3MGxogwX/ztb. </td>
	</tr>
	<tr class="row35">
		<td class="col0"> 1700 </td><td class="col1"> SHA-512 </td><td class="col2"> 82a9dda829eb7f8ffe9fbe49e45d47d2dad9664fbb7adf72492e3c81ebd3e29134d9bc12212bf83c6840f10e8246b9db54a4859b7ccd0123d86e5872c1e5082f </td>
	</tr>
	<tr class="row36">
		<td class="col0"> 1710 </td><td class="col1"> sha512($pass.$salt) </td><td class="col2"> e5c3ede3e49fb86592fb03f471c35ba13e8d89b8ab65142c9a8fdafb635fa2223c24e5558fd9313e8995019dcbec1fb584146b7bb12685c7765fc8c0d51379fd:6352283260 </td>
	</tr>
	<tr class="row37">
		<td class="col0"> 1720 </td><td class="col1"> sha512($salt.$pass) </td><td class="col2"> 976b451818634a1e2acba682da3fd6efa72adf8a7a08d7939550c244b237c72c7d42367544e826c0c83fe5c02f97c0373b6b1386cc794bf0d21d2df01bb9c08a:2613516180127 </td>
	</tr>
	<tr class="row38">
		<td class="col0"> 1730 </td><td class="col1"> sha512(utf16le($pass).$salt) </td><td class="col2"> 13070359002b6fbb3d28e50fba55efcf3d7cc115fe6e3f6c98bf0e3210f1c6923427a1e1a3b214c1de92c467683f6466727ba3a51684022be5cc2ffcb78457d2:341351589 </td>
	</tr>
	<tr class="row39">
		<td class="col0"> 1740 </td><td class="col1"> sha512($salt.utf16le($pass)) </td><td class="col2"> bae3a3358b3459c761a3ed40d34022f0609a02d90a0d7274610b16147e58ece00cd849a0bd5cf6a92ee5eb5687075b4e754324dfa70deca6993a85b2ca865bc8:1237015423 </td>
	</tr>
	<tr class="row40">
		<td class="col0"> 1750 </td><td class="col1"> HMAC-SHA512 (key = $pass) </td><td class="col2"> 94cb9e31137913665dbea7b058e10be5f050cc356062a2c9679ed0ad6119648e7be620e9d4e1199220cd02b9efb2b1c78234fa1000c728f82bf9f14ed82c1976:1234 </td>
	</tr>
	<tr class="row41">
		<td class="col0"> 1760 </td><td class="col1"> HMAC-SHA512 (key = $salt) </td><td class="col2"> 7cce966f5503e292a51381f238d071971ad5442488f340f98e379b3aeae2f33778e3e732fcc2f7bdc04f3d460eebf6f8cb77da32df25500c09160dd3bf7d2a6b:1234 </td>
	</tr>
	<tr class="row42">
		<td class="col0"> 1800 </td><td class="col1"> sha512crypt $6$, SHA512 (Unix) <sup>2</sup> </td><td class="col2"> $6$52450745$k5ka2p8bFuSmoVT1tzOyyuaREkkKBcCNqoDKzYiJL9RaE8yMnPgh2XzzF0NDrUhgrcLwg78xs1w5pJiypEdFX/ </td>
	</tr>
	<tr class="row43">
		<td class="col0"> 2000 </td><td class="col1"> STDOUT </td><td class="col2"> n/a </td>
	</tr>
	<tr class="row44">
		<td class="col0"> 2100 </td><td class="col1"> Domain Cached Credentials 2 (DCC2), MS Cache 2 </td><td class="col2 leftalign"> $DCC2$10240#tom#e4e938d12fe5974dc42a90120bd9c90f  </td>
	</tr>
	<tr class="row45">
		<td class="col0"> 2400 </td><td class="col1"> Cisco-PIX MD5 </td><td class="col2"> dRRVnUmUHXOTt9nk </td>
	</tr>
	<tr class="row46">
		<td class="col0"> 2410 </td><td class="col1"> Cisco-ASA MD5 </td><td class="col2"> 02dMBMYkTdC5Ziyp:36 </td>
	</tr>
	<tr class="row47">
		<td class="col0"> 2500 </td><td class="col1"> WPA/WPA2 <sup>1</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.hccapx" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.hccapx" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.hccapx</a> </td>
	</tr>
	<tr class="row48">
		<td class="col0"> 2501 </td><td class="col1"> WPA/WPA2 PMK <sup>14</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat-pmk.hccapx" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat-pmk.hccapx" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat-pmk.hccapx</a> </td>
	</tr>
	<tr class="row49">
		<td class="col0"> 2600 </td><td class="col1"> md5(md5($pass)) </td><td class="col2"> a936af92b0ae20b1ff6c3347a72e5fbe </td>
	</tr>
	<tr class="row50">
		<td class="col0"> 3000 </td><td class="col1"> LM </td><td class="col2"> 299bd128c1101fd6 </td>
	</tr>
	<tr class="row51">
		<td class="col0"> 3100 </td><td class="col1"> Oracle H: Type (Oracle 7+), DES(Oracle) </td><td class="col2"> 7A963A529D2E3229:3682427524 </td>
	</tr>
	<tr class="row52">
		<td class="col0"> 3200 </td><td class="col1"> bcrypt $2*$, Blowfish (Unix) </td><td class="col2"> $2a$05$LhayLxezLhK1LhWvKxCyLOj0j1u.Kj0jZ0pEmm134uzrQlFvQJLF6 </td>
	</tr>
	<tr class="row53">
		<td class="col0"> 3710 </td><td class="col1"> md5($salt.md5($pass)) </td><td class="col2"> 95248989ec91f6d0439dbde2bd0140be:1234 </td>
	</tr>
	<tr class="row54">
		<td class="col0"> 3800 </td><td class="col1"> md5($salt.$pass.$salt) </td><td class="col2"> 2e45c4b99396c6cb2db8bda0d3df669f:1234 </td>
	</tr>
	<tr class="row55">
		<td class="col0"> 3910 </td><td class="col1"> md5(md5($pass).md5($salt)) </td><td class="col2"> 250920b3a5e31318806a032a4674df7e:1234 </td>
	</tr>
	<tr class="row56">
		<td class="col0"> 4010 </td><td class="col1"> md5($salt.md5($salt.$pass)) </td><td class="col2"> 30d0cf4a5d7ed831084c5b8b0ba75b46:1234 </td>
	</tr>
	<tr class="row57">
		<td class="col0"> 4110 </td><td class="col1"> md5($salt.md5($pass.$salt)) </td><td class="col2"> b4cb5c551a30f6c25d648560408df68a:1234 </td>
	</tr>
	<tr class="row58">
		<td class="col0"> 4300 </td><td class="col1"> md5(strtoupper(md5($pass))) </td><td class="col2"> b8c385461bb9f9d733d3af832cf60b27 </td>
	</tr>
	<tr class="row59">
		<td class="col0"> 4400 </td><td class="col1"> md5(sha1($pass)) </td><td class="col2"> 288496df99b33f8f75a7ce4837d1b480 </td>
	</tr>
	<tr class="row60">
		<td class="col0"> 4500 </td><td class="col1"> sha1(sha1($pass)) </td><td class="col2"> 3db9184f5da4e463832b086211af8d2314919951 </td>
	</tr>
	<tr class="row61">
		<td class="col0"> 4520 </td><td class="col1"> sha1($salt.sha1($pass)) </td><td class="col2"> a0f835fdf57d36ebd8d0399cc44e6c2b86a1072b:511358214352751667201107073531735211566650747315 </td>
	</tr>
	<tr class="row62">
		<td class="col0"> 4700 </td><td class="col1"> sha1(md5($pass)) </td><td class="col2"> 92d85978d884eb1d99a51652b1139c8279fa8663 </td>
	</tr>
	<tr class="row63">
		<td class="col0"> 4710 </td><td class="col1"> sha1(md5($pass).$salt) <sup>*</sup> </td><td class="col2"> 53c724b7f34f09787ed3f1b316215fc35c789504:hashcat1 </td>
	</tr>
	<tr class="row64">
		<td class="col0"> 4800 </td><td class="col1"> iSCSI CHAP authentication, MD5(CHAP) <sup>7</sup> </td><td class="col2"> afd09efdd6f8ca9f18ec77c5869788c3:01020304050607080910111213141516:01 </td>
	</tr>
	<tr class="row65">
		<td class="col0"> 4900 </td><td class="col1"> sha1($salt.$pass.$salt) </td><td class="col2"> 85087a691a55cbb41ae335d459a9121d54080b80:488387841 </td>
	</tr>
	<tr class="row66">
		<td class="col0"> 5100 </td><td class="col1"> Half MD5 </td><td class="col2"> 8743b52063cd8409 </td>
	</tr>
	<tr class="row67">
		<td class="col0"> 5200 </td><td class="col1"> Password Safe v3 </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.psafe3" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.psafe3" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.psafe3</a> </td>
	</tr>
	<tr class="row68">
		<td class="col0"> 5300 </td><td class="col1"> IKE-PSK MD5 </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.ikemd5" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.ikemd5" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.ikemd5</a> </td>
	</tr>
	<tr class="row69">
		<td class="col0"> 5400 </td><td class="col1"> IKE-PSK SHA1 </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.ikesha1" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.ikesha1" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.ikesha1</a> </td>
	</tr>
	<tr class="row70">
		<td class="col0"> 5500 </td><td class="col1"> NetNTLMv1 / NetNTLMv1+ESS </td><td class="col2"> u4-netntlm::kNS:338d08f8e26de93300000000000000000000000000000000:9526fb8c23a90751cdd619b6cea564742e1e4bf33006ba41:cb8086049ec4736c </td>
	</tr>
	<tr class="row71">
		<td class="col0"> 5600 </td><td class="col1"> NetNTLMv2 </td><td class="col2"> admin::N46iSNekpT:08ca45b7d7ea58ee:88dcbe4446168966a153a0064958dac6:5c7830315c7830310000000000000b45c67103d07d7b95acd12ffa11230e0000000052920b85f78d013c31cdb3b92f5d765c783030 </td>
	</tr>
	<tr class="row72">
		<td class="col0"> 5700 </td><td class="col1"> Cisco-IOS type 4 (SHA256) </td><td class="col2"> 2btjjy78REtmYkkW0csHUbJZOstRXoWdX1mGrmmfeHI </td>
	</tr>
	<tr class="row73">
		<td class="col0"> 5800 </td><td class="col1"> Samsung Android Password/PIN </td><td class="col2"> 0223b799d526b596fe4ba5628b9e65068227e68e:f6d45822728ddb2c </td>
	</tr>
	<tr class="row74">
		<td class="col0"> 6000 </td><td class="col1"> RIPEMD-160 </td><td class="col2"> 012cb9b334ec1aeb71a9c8ce85586082467f7eb6 </td>
	</tr>
	<tr class="row75">
		<td class="col0"> 6100 </td><td class="col1"> Whirlpool </td><td class="col2"> 7ca8eaaaa15eaa4c038b4c47b9313e92da827c06940e69947f85bc0fbef3eb8fd254da220ad9e208b6b28f6bb9be31dd760f1fdb26112d83f87d96b416a4d258 </td>
	</tr>
	<tr class="row76">
		<td class="col0"> 6211 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes.tc</a> </td>
	</tr>
	<tr class="row77">
		<td class="col0"> 6211 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent.tc</a> </td>
	</tr>
	<tr class="row78">
		<td class="col0"> 6211 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish.tc</a> </td>
	</tr>
	<tr class="row79">
		<td class="col0"> 6212 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish.tc</a> </td>
	</tr>
	<tr class="row80">
		<td class="col0"> 6213 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES-Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row81">
		<td class="col0"> 6212 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes.tc</a> </td>
	</tr>
	<tr class="row82">
		<td class="col0"> 6213 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes.tc</a> </td>
	</tr>
	<tr class="row83">
		<td class="col0"> 6212 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row84">
		<td class="col0"> 6221 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_aes.tc</a> </td>
	</tr>
	<tr class="row85">
		<td class="col0"> 6221 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent.tc</a> </td>
	</tr>
	<tr class="row86">
		<td class="col0"> 6221 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish.tc</a> </td>
	</tr>
	<tr class="row87">
		<td class="col0"> 6222 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish.tc</a> </td>
	</tr>
	<tr class="row88">
		<td class="col0"> 6223 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + AES-Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_aes-twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row89">
		<td class="col0"> 6222 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-aes.tc</a> </td>
	</tr>
	<tr class="row90">
		<td class="col0"> 6223 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-twofish-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-twofish-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_serpent-twofish-aes.tc</a> </td>
	</tr>
	<tr class="row91">
		<td class="col0"> 6222 </td><td class="col1"> TrueCrypt 5.0+ SHA512 + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_sha512_twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row92">
		<td class="col0"> 6231 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes.tc</a> </td>
	</tr>
	<tr class="row93">
		<td class="col0"> 6231 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent.tc</a> </td>
	</tr>
	<tr class="row94">
		<td class="col0"> 6231 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish.tc</a> </td>
	</tr>
	<tr class="row95">
		<td class="col0"> 6232 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish.tc</a> </td>
	</tr>
	<tr class="row96">
		<td class="col0"> 6233 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + AES-Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_aes-twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row97">
		<td class="col0"> 6232 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-aes.tc</a> </td>
	</tr>
	<tr class="row98">
		<td class="col0"> 6233 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-twofish-aes.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-twofish-aes.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_serpent-twofish-aes.tc</a> </td>
	</tr>
	<tr class="row99">
		<td class="col0"> 6232 </td><td class="col1"> TrueCrypt 5.0+ Whirlpool + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish-serpent.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish-serpent.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_whirlpool_twofish-serpent.tc</a> </td>
	</tr>
	<tr class="row100">
		<td class="col0"> 6241 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes_boot.tc</a> </td>
	</tr>
	<tr class="row101">
		<td class="col0"> 6241 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent_boot.tc</a> </td>
	</tr>
	<tr class="row102">
		<td class="col0"> 6241 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Twofish + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish_boot.tc</a> </td>
	</tr>
	<tr class="row103">
		<td class="col0"> 6242 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES-Twofish + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish_boot.tc</a> </td>
	</tr>
	<tr class="row104">
		<td class="col0"> 6243 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + AES-Twofish-Serpent + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_aes-twofish-serpent_boot.tc</a> </td>
	</tr>
	<tr class="row105">
		<td class="col0"> 6242 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent-AES + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-aes_boot.tc</a> </td>
	</tr>
	<tr class="row106">
		<td class="col0"> 6243 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Serpent-Twofish-AES + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_serpent-twofish-aes_boot.tc</a> </td>
	</tr>
	<tr class="row107">
		<td class="col0"> 6242 </td><td class="col1"> TrueCrypt 5.0+ PBKDF2-HMAC-RIPEMD160 + Twofish-Serpent + boot </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent_boot.tc" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent_boot.tc" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_ripemd160_twofish-serpent_boot.tc</a> </td>
	</tr>
	<tr class="row108">
		<td class="col0"> 6300 </td><td class="col1"> AIX {smd5} </td><td class="col2"> {smd5}a5/yTL/u$VfvgyHx1xUlXZYBocQpQY0 </td>
	</tr>
	<tr class="row109">
		<td class="col0"> 6400 </td><td class="col1"> AIX {ssha256} </td><td class="col2"> {ssha256}06$aJckFGJAB30LTe10$ohUsB7LBPlgclE3hJg9x042DLJvQyxVCX.nZZLEz.g2 </td>
	</tr>
	<tr class="row110">
		<td class="col0"> 6500 </td><td class="col1 leftalign"> AIX {ssha512}  </td><td class="col2">{ssha512}06$bJbkFGJAB30L2e23$bXiXjyH5YGIyoWWmEVwq67nCU5t7GLy9HkCzrodRCQCx3r9VvG98o7O3V0r9cVrX3LPPGuHqT5LLn0oGCuI1.. </td>
	</tr>
	<tr class="row111">
		<td class="col0"> 6600 </td><td class="col1"> 1Password, agilekeychain </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.agilekeychain" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.agilekeychain" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.agilekeychain</a> </td>
	</tr>
	<tr class="row112">
		<td class="col0"> 6700 </td><td class="col1"> AIX {ssha1} </td><td class="col2"> {ssha1}06$bJbkFGJAB30L2e23$dCESGOsP7jaIIAJ1QAcmaGeG.kr </td>
	</tr>
	<tr class="row113">
		<td class="col0"> 6800 </td><td class="col1"> LastPass + LastPass sniffed<sup>4</sup> </td><td class="col2"> a2d1f7b7a1862d0d4a52644e72d59df5:500:lp@trash-mail.com </td>
	</tr>
	<tr class="row114">
		<td class="col0"> 6900 </td><td class="col1"> GOST R 34.11-94 </td><td class="col2"> df226c2c6dcb1d995c0299a33a084b201544293c31fc3d279530121d36bbcea9 </td>
	</tr>
	<tr class="row115">
		<td class="col0"> 7000 </td><td class="col1"> FortiGate (FortiOS) </td><td class="col2"> AK1AAECAwQFBgcICRARNGqgeC3is8gv2xWWRony9NJnDgE= </td>
	</tr>
	<tr class="row116">
		<td class="col0"> 7100 </td><td class="col1"> OSX v10.8+ (PBKDF2-SHA512) </td><td class="col2"> $ml$35460$93a94bd24b5de64d79a5e49fa372827e739f4d7b6975c752c9a0ff1e5cf72e05$752351df64dd2ce9dc9c64a72ad91de6581a15c19176266b44d98919dfa81f0f96cbcb20a1ffb400718c20382030f637892f776627d34e021bad4f81b7de8222 </td>
	</tr>
	<tr class="row117">
		<td class="col0"> 7200 </td><td class="col1"> GRUB 2 </td><td class="col2"> grub.pbkdf2.sha512.10000.7d391ef48645f626b427b1fae06a7219b5b54f4f02b2621f86b5e36e83ae492bd1db60871e45bc07925cecb46ff8ba3db31c723c0c6acbd4f06f60c5b246ecbf.26d59c52b50df90d043f070bd9cbcd92a74424da42b3666fdeb08f1a54b8f1d2f4f56cf436f9382419c26798dc2c209a86003982b1e5a9fcef905f4dfaa4c524 </td>
	</tr>
	<tr class="row118">
		<td class="col0"> 7300 </td><td class="col1"> IPMI2 RAKP HMAC-SHA1 </td><td class="col2"> b7c2d6f13a43dce2e44ad120a9cd8a13d0ca23f0414275c0bbe1070d2d1299b1c04da0f1a0f1e4e2537300263a2200000000000000000000140768617368636174:472bdabe2d5d4bffd6add7b3ba79a291d104a9ef </td>
	</tr>
	<tr class="row119">
		<td class="col0"> 7400 </td><td class="col1"> sha256crypt $5$, SHA256 (Unix) <sup>2</sup> </td><td class="col2"> $5$rounds=5000$GX7BopJZJxPc/KEK$le16UF8I2Anb.rOrn22AUPWvzUETDGefUmAV8AZkGcD </td>
	</tr>
	<tr class="row120">
		<td class="col0"> 7500 </td><td class="col1"> Kerberos 5 AS-REQ Pre-Auth etype 23 </td><td class="col2"> $krb5pa$23$user$realm$salt$4e751db65422b2117f7eac7b721932dc8aa0d9966785ecd958f971f622bf5c42dc0c70b532363138363631363132333238383835 </td>
	</tr>
	<tr class="row121">
		<td class="col0"> 7700 </td><td class="col1"> SAP CODVN B (BCODE) </td><td class="col2"> USER$C8B48F26B87B7EA7 </td>
	</tr>
	<tr class="row122">
		<td class="col0"> 7701 </td><td class="col1"> SAP CODVN B (BCODE) mangled from <abbr title="Request for Comments">RFC</abbr>_READ_TABLE </td><td class="col2"> 027642760180$77EC386300000000 </td>
	</tr>
	<tr class="row123">
		<td class="col0"> 7800 </td><td class="col1"> SAP CODVN F/G (PASSCODE) </td><td class="col2"> USER$ABCAD719B17E7F794DF7E686E563E9E2D24DE1D0 </td>
	</tr>
	<tr class="row124">
		<td class="col0"> 7801 </td><td class="col1"> SAP CODVN F/G (PASSCODE) mangled from <abbr title="Request for Comments">RFC</abbr>_READ_TABLE </td><td class="col2"> 604020408266$32837BA7B97672BA4E5A00000000000000000000 </td>
	</tr>
	<tr class="row125">
		<td class="col0"> 7900 </td><td class="col1"> Drupal7 </td><td class="col2"> $S$C33783772bRXEx1aCsvY.dqgaaSu76XmVlKrW9Qu8IQlvxHlmzLf </td>
	</tr>
	<tr class="row126">
		<td class="col0"> 8000 </td><td class="col1"> Sybase ASE </td><td class="col2"> 0xc00778168388631428230545ed2c976790af96768afa0806fe6c0da3b28f3e132137eac56f9bad027ea2 </td>
	</tr>
	<tr class="row127">
		<td class="col0"> 8100 </td><td class="col1"> Citrix NetScaler </td><td class="col2"> 1765058016a22f1b4e076dccd1c3df4e8e5c0839ccded98ea </td>
	</tr>
	<tr class="row128">
		<td class="col0"> 8200 </td><td class="col1"> 1Password, cloudkeychain </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.cloudkeychain" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.cloudkeychain" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.cloudkeychain</a> </td>
	</tr>
	<tr class="row129">
		<td class="col0"> 8300 </td><td class="col1"> DNSSEC (NSEC3) </td><td class="col2"> 7b5n74kq8r441blc2c5qbbat19baj79r:.lvdsiqfj.net:33164473:1 </td>
	</tr>
	<tr class="row130">
		<td class="col0"> 8400 </td><td class="col1"> WBB3 (Woltlab Burning Board) </td><td class="col2"> 8084df19a6dc81e2597d051c3d8b400787e2d5a9:6755045315424852185115352765375338838643 </td>
	</tr>
	<tr class="row131">
		<td class="col0"> 8500 </td><td class="col1"> RACF </td><td class="col2"> $racf$*USER*FC2577C6EBE6265B </td>
	</tr>
	<tr class="row132">
		<td class="col0"> 8600 </td><td class="col1"> Lotus Notes/Domino 5 </td><td class="col2"> 3dd2e1e5ac03e230243d58b8c5ada076 </td>
	</tr>
	<tr class="row133">
		<td class="col0"> 8700 </td><td class="col1"> Lotus Notes/Domino 6 </td><td class="col2"> (GDpOtD35gGlyDksQRxEU) </td>
	</tr>
	<tr class="row134">
		<td class="col0"> 8800 </td><td class="col1"> Android FDE &lt;= 4.3 </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.android43fde" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.android43fde" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.android43fde</a> </td>
	</tr>
	<tr class="row135">
		<td class="col0"> 8900 </td><td class="col1"> scrypt </td><td class="col2"> SCRYPT:1024:1:1:MDIwMzMwNTQwNDQyNQ==:5FW+zWivLxgCWj7qLiQbeC8zaNQ+qdO0NUinvqyFcfo= </td>
	</tr>
	<tr class="row136">
		<td class="col0"> 9000 </td><td class="col1"> Password Safe v2 </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat.psafe2.dat" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat.psafe2.dat" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat.psafe2.dat</a> </td>
	</tr>
	<tr class="row137">
		<td class="col0"> 9100 </td><td class="col1"> Lotus Notes/Domino 8 </td><td class="col2"> (HsjFebq0Kh9kH7aAZYc7kY30mC30mC3KmC30mCluagXrvWKj1) </td>
	</tr>
	<tr class="row138">
		<td class="col0"> 9200 </td><td class="col1"> Cisco-IOS $8$ (PBKDF2-SHA256) </td><td class="col2 leftalign"> $8$TnGX/fE4KGHOVU$pEhnEvxrvaynpi8j4f.EMHr6M.FzU8xnZnBr/tJdFWk  </td>
	</tr>
	<tr class="row139">
		<td class="col0"> 9300 </td><td class="col1"> Cisco-IOS $9$ (scrypt) </td><td class="col2 leftalign"> $9$2MJBozw/9R3UsU$2lFhcKvpghcyw8deP25GOfyZaagyUOGBymkryvOdfo6  </td>
	</tr>
	<tr class="row140">
		<td class="col0"> 9400 </td><td class="col1"> MS Office 2007 </td><td class="col2"> $office$*2007*20*128*16*411a51284e0d0200b131a8949aaaa5cc*117d532441c63968bee7647d9b7df7d6*df1d601ccf905b375575108f42ef838fb88e1cde </td>
	</tr>
	<tr class="row141">
		<td class="col0"> 9500 </td><td class="col1"> MS Office 2010 </td><td class="col2 leftalign"> $office$*2010*100000*128*16*77233201017277788267221014757262*b2d0ca4854ba19cf95a2647d5eee906c*e30cbbb189575cafb6f142a90c2622fa9e78d293c5b0c001517b3f5b82993557  </td>
	</tr>
	<tr class="row142">
		<td class="col0"> 9600 </td><td class="col1"> MS Office 2013 </td><td class="col2 leftalign"> $office$*2013*100000*256*16*7dd611d7eb4c899f74816d1dec817b3b*948dc0b2c2c6c32f14b5995a543ad037*0b7ee0e48e935f937192a59de48a7d561ef2691d5c8a3ba87ec2d04402a94895  </td>
	</tr>
	<tr class="row143">
		<td class="col0"> 9700 </td><td class="col1"> MS Office ⇐ 2003 MD5 + RC4, oldoffice$0, oldoffice$1 </td><td class="col2"> $oldoffice$1*04477077758555626246182730342136*b1b72ff351e41a7c68f6b45c4e938bd6*0d95331895e99f73ef8b6fbc4a78ac1a </td>
	</tr>
	<tr class="row144">
		<td class="col0"> 9710 </td><td class="col1"> MS Office ⇐ 2003 $0/$1, MD5 + RC4, collider #1 </td><td class="col2"> $oldoffice$0*55045061647456688860411218030058*e7e24d163fbd743992d4b8892bf3f2f7*493410dbc832557d3fe1870ace8397e2 </td>
	</tr>
	<tr class="row145">
		<td class="col0"> 9720 </td><td class="col1"> MS Office ⇐ 2003 $0/$1, MD5 + RC4, collider #2 </td><td class="col2"> $oldoffice$0*55045061647456688860411218030058*e7e24d163fbd743992d4b8892bf3f2f7*493410dbc832557d3fe1870ace8397e2:91b2e062b9 </td>
	</tr>
	<tr class="row146">
		<td class="col0"> 9800 </td><td class="col1"> MS Office ⇐ 2003 SHA1 + RC4, oldoffice$3, oldoffice$4 </td><td class="col2"> $oldoffice$3*83328705222323020515404251156288*2855956a165ff6511bc7f4cd77b9e101*941861655e73a09c40f7b1e9dfd0c256ed285acd </td>
	</tr>
	<tr class="row147">
		<td class="col0"> 9810 </td><td class="col1"> MS Office ⇐ 2003 $3, SHA1 + RC4, collider #1 </td><td class="col2"> $oldoffice$3*83328705222323020515404251156288*2855956a165ff6511bc7f4cd77b9e101*941861655e73a09c40f7b1e9dfd0c256ed285acd </td>
	</tr>
	<tr class="row148">
		<td class="col0"> 9820 </td><td class="col1"> MS Office ⇐ 2003 $3, SHA1 + RC4, collider #2 </td><td class="col2"> $oldoffice$3*83328705222323020515404251156288*2855956a165ff6511bc7f4cd77b9e101*941861655e73a09c40f7b1e9dfd0c256ed285acd:b8f63619ca </td>
	</tr>
	<tr class="row149">
		<td class="col0"> 9900 </td><td class="col1"> Radmin2 </td><td class="col2"> 22527bee5c29ce95373c4e0f359f079b </td>
	</tr>
	<tr class="row150">
		<td class="col0"> 10000 </td><td class="col1"> Django (PBKDF2-SHA256) </td><td class="col2"> pbkdf2_sha256$20000$H0dPx8NeajVu$GiC4k5kqbbR9qWBlsRgDywNqC2vd9kqfk7zdorEnNas= </td>
	</tr>
	<tr class="row151">
		<td class="col0"> 10100 </td><td class="col1"> SipHash </td><td class="col2"> ad61d78c06037cd9:2:4:81533218127174468417660201434054 </td>
	</tr>
	<tr class="row152">
		<td class="col0"> 10200 </td><td class="col1"> CRAM-MD5 </td><td class="col2"> $cram_md5$PG5vLXJlcGx5QGhhc2hjYXQubmV0Pg==$dXNlciA0NGVhZmQyMmZlNzY2NzBmNmIyODc5MDgxYTdmNWY3MQ== </td>
	</tr>
	<tr class="row153">
		<td class="col0"> 10300 </td><td class="col1"> SAP CODVN H (PWDSALTEDHASH) iSSHA-1 </td><td class="col2"> {x-issha, 1024}C0624EvGSdAMCtuWnBBYBGA0chvqAflKY74oEpw/rpY= </td>
	</tr>
	<tr class="row154">
		<td class="col0"> 10400 </td><td class="col1"> PDF 1.1 - 1.3 (Acrobat 2 - 4) </td><td class="col2"> $pdf$1*2*40*-1*0*16*51726437280452826511473255744374*32*9b09be05c226214fa1178342673d86f273602b95104f2384b6c9b709b2cbc058*32*0000000000000000000000000000000000000000000000000000000000000000 </td>
	</tr>
	<tr class="row155">
		<td class="col0"> 10410 </td><td class="col1"> PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #1 </td><td class="col2"> $pdf$1*2*40*-1*0*16*01221086741440841668371056103222*32*27c3fecef6d46a78eb61b8b4dbc690f5f8a2912bbb9afc842c12d79481568b74*32*0000000000000000000000000000000000000000000000000000000000000000 </td>
	</tr>
	<tr class="row156">
		<td class="col0"> 10420 </td><td class="col1"> PDF 1.1 - 1.3 (Acrobat 2 - 4), collider #2 </td><td class="col2"> $pdf$1*2*40*-1*0*16*01221086741440841668371056103222*32*27c3fecef6d46a78eb61b8b4dbc690f5f8a2912bbb9afc842c12d79481568b74*32*0000000000000000000000000000000000000000000000000000000000000000:6a8aedccb7 </td>
	</tr>
	<tr class="row157">
		<td class="col0"> 10500 </td><td class="col1"> PDF 1.4 - 1.6 (Acrobat 5 - 8) </td><td class="col2"> $pdf$2*3*128*-1028*1*16*da42ee15d4b3e08fe5b9ecea0e02ad0f*32*c9b59d72c7c670c42eeb4fca1d2ca15000000000000000000000000000000000*32*c4ff3e868dc87604626c2b8c259297a14d58c6309c70b00afdfb1fbba10ee571 </td>
	</tr>
	<tr class="row158">
		<td class="col0"> 10600 </td><td class="col1"> PDF 1.7 Level 3 (Acrobat 9) </td><td class="col2"> $pdf$5*5*256*-1028*1*16*20583814402184226866485332754315*127*f95d927a94829db8e2fbfbc9726ebe0a391b22a084ccc2882eb107a74f7884812058381440218422686648533275431500000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000*127*00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000*32*0000000000000000000000000000000000000000000000000000000000000000*32*0000000000000000000000000000000000000000000000000000000000000000 </td>
	</tr>
	<tr class="row159">
		<td class="col0"> 10700 </td><td class="col1"> PDF 1.7 Level 8 (Acrobat 10 - 11) </td><td class="col2"> $pdf$5*6*256*-1028*1*16*21240790753544575679622633641532*127*2d1ecff66ea354d3d34325a6503da57e03c199c21b13dd842f8d515826054d8d2124079075354457567962263364153200000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000*127*00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000*32*0000000000000000000000000000000000000000000000000000000000000000*32*0000000000000000000000000000000000000000000000000000000000000000 </td>
	</tr>
	<tr class="row160">
		<td class="col0"> 10800 </td><td class="col1"> SHA-384 </td><td class="col2"> 07371af1ca1fca7c6941d2399f3610f1e392c56c6d73fddffe38f18c430a2817028dae1ef09ac683b62148a2c8757f42 </td>
	</tr>
	<tr class="row161">
		<td class="col0"> 10900 </td><td class="col1"> PBKDF2-HMAC-SHA256 </td><td class="col2"> sha256:1000:MTc3MTA0MTQwMjQxNzY=:PYjCU215Mi57AYPKva9j7mvF4Rc5bCnt </td>
	</tr>
	<tr class="row162">
		<td class="col0"> 11000 </td><td class="col1"> PrestaShop </td><td class="col2"> 810e3d12f0f10777a679d9ca1ad7a8d9:M2uZ122bSHJ4Mi54tXGY0lqcv1r28mUluSkyw37ou5oia4i239ujqw0l </td>
	</tr>
	<tr class="row163">
		<td class="col0"> 11100 </td><td class="col1"> PostgreSQL CRAM (MD5) </td><td class="col2"> $postgres$postgres*f0784ea5*2091bb7d4725d1ca85e8de6ec349baf6 </td>
	</tr>
	<tr class="row164">
		<td class="col0"> 11200 </td><td class="col1"> MySQL CRAM (SHA1) </td><td class="col2"> $mysqlna$1c24ab8d0ee94d70ab1f2e814d8f0948a14d10b9*437e93572f18ae44d9e779160c2505271f85821d </td>
	</tr>
	<tr class="row165">
		<td class="col0"> 11300 </td><td class="col1"> Bitcoin/Litecoin wallet.dat </td><td class="col2"> $bitcoin$96$d011a1b6a8d675b7a36d0cd2efaca32a9f8dc1d57d6d01a58399ea04e703e8bbb44899039326f7a00f171a7bbc854a54$16$1563277210780230$158555$96$628835426818227243334570448571536352510740823233055715845322741625407685873076027233865346542174$66$625882875480513751851333441623702852811440775888122046360561760525 </td>
	</tr>
	<tr class="row166">
		<td class="col0"> 11400 </td><td class="col1"> SIP digest authentication (MD5) </td><td class="col2"> $sip$*192.168.100.100*192.168.100.121*username*asterisk*REGISTER*sip*192.168.100.121**2b01df0b****MD5*ad0520061ca07c120d7e8ce696a6df2d </td>
	</tr>
	<tr class="row167">
		<td class="col0"> 11500 </td><td class="col1"> CRC32 <sup>5</sup> </td><td class="col2"> c762de4a:00000000 </td>
	</tr>
	<tr class="row168">
		<td class="col0"> 11600 </td><td class="col1"> 7-Zip </td><td class="col2"> $7z$0$19$0$salt$8$f6196259a7326e3f0000000000000000$185065650$112$98$f3bc2a88062c419a25acd40c0c2d75421cf23263f69c51b13f9b1aada41a8a09f9adeae45d67c60b56aad338f20c0dcc5eb811c7a61128ee0746f922cdb9c59096869f341c7a9cb1ac7bb7d771f546b82cf4e6f11a5ecd4b61751e4d8de66dd6e2dfb5b7d1022d2211e2d66ea1703f96 </td>
	</tr>
	<tr class="row169">
		<td class="col0"> 11700 </td><td class="col1"> GOST R 34.11-2012 (Streebog) 256-bit </td><td class="col2"> 57e9e50caec93d72e9498c211d6dc4f4d328248b48ecf46ba7abfa874f666e36 </td>
	</tr>
	<tr class="row170">
		<td class="col0"> 11750 </td><td class="col1"> HMAC-Streebog-256 (key = $pass), big-endian </td><td class="col2"> 0f71c7c82700c9094ca95eee3d804cc283b538bec49428a9ef8da7b34effb3ba:08151337 </td>
	</tr>
	<tr class="row171">
		<td class="col0"> 11760 </td><td class="col1"> HMAC-Streebog-256 (key = $salt), big-endian </td><td class="col2"> d5c6b874338a492ac57ddc6871afc3c70dcfd264185a69d84cf839a07ef92b2c:08151337 </td>
	</tr>
	<tr class="row172">
		<td class="col0"> 11800 </td><td class="col1"> GOST R 34.11-2012 (Streebog) 512-bit </td><td class="col2"> 5d5bdba48c8f89ee6c0a0e11023540424283e84902de08013aeeb626e819950bb32842903593a1d2e8f71897ff7fe72e17ac9ba8ce1d1d2f7e9c4359ea63bdc3 </td>
	</tr>
	<tr class="row173">
		<td class="col0"> 11850 </td><td class="col1"> HMAC-Streebog-512 (key = $pass), big-endian </td><td class="col2"> be4555415af4a05078dcf260bb3c0a35948135df3dbf93f7c8b80574ceb0d71ea4312127f839b7707bf39ccc932d9e7cb799671183455889e8dde3738dfab5b6:08151337 </td>
	</tr>
	<tr class="row174">
		<td class="col0"> 11860 </td><td class="col1"> HMAC-Streebog-512 (key = $salt), big-endian </td><td class="col2"> bebf6831b3f9f958acb345a88cb98f30cb0374cff13e6012818487c8dc8d5857f23bca2caed280195ad558b8ce393503e632e901e8d1eb2ccb349a544ac195fd:08151337 </td>
	</tr>
	<tr class="row175">
		<td class="col0"> 11900 </td><td class="col1"> PBKDF2-HMAC-MD5 </td><td class="col2"> md5:1000:MTg1MzA=:Lz84VOcrXd699Edsj34PP98+f4f3S0rTZ4kHAIHoAjs= </td>
	</tr>
	<tr class="row176">
		<td class="col0"> 12000 </td><td class="col1"> PBKDF2-HMAC-SHA1 </td><td class="col2"> sha1:1000:MzU4NTA4MzIzNzA1MDQ=:19ofiY+ahBXhvkDsp0j2ww== </td>
	</tr>
	<tr class="row177">
		<td class="col0"> 12100 </td><td class="col1"> PBKDF2-HMAC-SHA512 </td><td class="col2"> sha512:1000:ODQyMDEwNjQyODY=:MKaHNWXUsuJB3IEwBHbm3w== </td>
	</tr>
	<tr class="row178">
		<td class="col0"> 12200 </td><td class="col1"> eCryptfs </td><td class="col2"> $ecryptfs$0$1$7c95c46e82f364b3$60bba503f0a42d0c </td>
	</tr>
	<tr class="row179">
		<td class="col0"> 12300 </td><td class="col1"> Oracle T: Type (Oracle 12+) </td><td class="col2"> 78281A9C0CF626BD05EFC4F41B515B61D6C4D95A250CD4A605CA0EF97168D670EBCB5673B6F5A2FB9CC4E0C0101E659C0C4E3B9B3BEDA846CD15508E88685A2334141655046766111066420254008225 </td>
	</tr>
	<tr class="row180">
		<td class="col0"> 12400 </td><td class="col1"> BSDiCrypt, Extended DES </td><td class="col2"> _9G..8147mpcfKT8g0U. </td>
	</tr>
	<tr class="row181">
		<td class="col0"> 12500 </td><td class="col1"> RAR3-hp </td><td class="col2"> $RAR3$*0*45109af8ab5f297a*adbf6c5385d7a40373e8f77d7b89d317 </td>
	</tr>
	<tr class="row182">
		<td class="col0"> 12600 </td><td class="col1"> ColdFusion 10+ </td><td class="col2"> aee9edab5653f509c4c63e559a5e967b4c112273bc6bd84525e630a3f9028dcb:5136256866783777334574783782810410706883233321141647265340462733 </td>
	</tr>
	<tr class="row183">
		<td class="col0"> 12700 </td><td class="col1"> Blockchain, My Wallet </td><td class="col2"> $blockchain$288$5420055827231730710301348670802335e45a6f5f631113cb1148a6e96ce645ac69881625a115fd35256636d0908217182f89bdd53256a764e3552d3bfe68624f4f89bb6de60687ff1ebb3cbf4e253ee3bea0fe9d12d6e8325ddc48cc924666dc017024101b7dfb96f1f45cfcf642c45c83228fe656b2f88897ced2984860bf322c6a89616f6ea5800aadc4b293ddd46940b3171a40e0cca86f66f0d4a487aa3a1beb82569740d3bc90bc1cb6b4a11bc6f0e058432cc193cb6f41e60959d03a84e90f38e54ba106fb7e2bfe58ce39e0397231f7c53a4ed4fd8d2e886de75d2475cc8fdc30bf07843ed6e3513e218e0bb75c04649f053a115267098251fd0079272ec023162505725cc681d8be12507c2d3e1c9520674c68428df1739944b8ac </td>
	</tr>
	<tr class="row184">
		<td class="col0"> 12800 </td><td class="col1"> MS-AzureSync PBKDF2-HMAC-SHA256 </td><td class="col2"> v1;PPH1_MD4,84840328224366186645,100,005a491d8bf3715085d69f934eef7fb19a15ffc233b5382d9827910bc32f3506 </td>
	</tr>
	<tr class="row185">
		<td class="col0"> 12900 </td><td class="col1"> Android FDE (Samsung DEK) </td><td class="col2"> 38421854118412625768408160477112384218541184126257684081604771129b6258eb22fc8b9d08e04e6450f72b98725d7d4fcad6fb6aec4ac2a79d0c6ff738421854118412625768408160477112 </td>
	</tr>
	<tr class="row186">
		<td class="col0"> 13000 </td><td class="col1"> RAR5 </td><td class="col2"> $rar5$16$74575567518807622265582327032280$15$f8b4064de34ac02ecabfe9abdf93ed6a$8$9843834ed0f7c754 </td>
	</tr>
	<tr class="row187">
		<td class="col0"> 13100 </td><td class="col1"> Kerberos 5 TGS-REP etype 23 </td><td class="col2"> $krb5tgs$23$*user$realm$test/spn*$63386d22d359fe42230300d56852c9eb$891ad31d09ab89c6b3b8c5e5de6c06a7f49fd559d7a9a3c32576c8fedf705376cea582ab5938f7fc8bc741acf05c5990741b36ef4311fe3562a41b70a4ec6ecba849905f2385bb3799d92499909658c7287c49160276bca0006c350b0db4fd387adc27c01e9e9ad0c20ed53a7e6356dee2452e35eca2a6a1d1432796fc5c19d068978df74d3d0baf35c77de12456bf1144b6a750d11f55805f5a16ece2975246e2d026dce997fba34ac8757312e9e4e6272de35e20d52fb668c5ed </td>
	</tr>
	<tr class="row188">
		<td class="col0"> 13200 </td><td class="col1"> AxCrypt </td><td class="col2"> $axcrypt$*1*10000*aaf4a5b4a7185551fea2585ed69fe246*45c616e901e48c6cac7ff14e8cd99113393be259c595325e </td>
	</tr>
	<tr class="row189">
		<td class="col0"> 13300 </td><td class="col1"> AxCrypt in-memory SHA1 <sup>13</sup> </td><td class="col2"> $axcrypt_sha1$b89eaac7e61417341b710b727768294d0e6a277b </td>
	</tr>
	<tr class="row190">
		<td class="col0"> 13400 </td><td class="col1"> KeePass 1 AES / without keyfile </td><td class="col2"> $keepass$*1*50000*0*375756b9e6c72891a8e5645a3338b8c8*82afc053e8e1a6cfa39adae4f5fe5e59f545a54d6956593d1709b39cacd7f796*c698fbfc7d1b71431d10611e2216ab21*24a63140f4eb3bfd7d59b7694eea38d1d93a43bc3af989755d2b326286c4d510*1*192*1a65072f436e9da0c9e832eca225a04ab78821b55d9f550860ade2ef8126a2c4050cf4d033374abd3dac6d0c5907c6cbb033643b203825c12e6c9853b5ac17a4809559fe723e01b4a2ab87cc83c8ba7ee4a757b8a0cf1674106f21f6675cba12064443d65436650df10ea0923c4cadfd4bfe341a6f4fa23a1a67f7d12a489fc5410ef6db9f6607905de491d3b3b915852a1b6c231c96366cbdee5ea9bd7f73ffd2f7a579215528ae1bf0ea540947ebfe39ca84bc6cbeded4f8e8fb6ed8f32dd5 </td>
	</tr>
	<tr class="row191">
		<td class="col0"> 13400 </td><td class="col1"> KeePass 2 AES / without keyfile </td><td class="col2"> $keepass$*2*6000*222*a279e37c38b0124559a83fa452a0269d56dc4119a5866d18e76f1f3fd536d64d*7ec7a06bc975ea2ae7c8dcb99e826a308564849b6b25d858cbbc78475af3733f*d477c849bf2278b7a1f626c81e343553*38c8ec186141c2705f2bcb334a730933ed3b0ee11391e1100fbaf429f6c99078*1ada85fe78cf36ab0537562a787dd83e446f13cd3d9a60fd495003de3537b702 </td>
	</tr>
	<tr class="row192">
		<td class="col0"> 13400 </td><td class="col1"> KeePass 1 Twofish / with keyfile </td><td class="col2"> $keepass$*1*6000*1*31c087828b0bb76362c10cae773aacdf*6d6c78b4f82ecbcd3b96670cf490914c25ea8c31bc3aeb3fc56e65fac16d721f*a735ec88c01816bc66200c8e17ee9110*08334be8523f4b69bd4e2328db854329bfc81e2ea5a46d8ccf3bccf7c03d879d*1*1360*f1e2c6c47f88c2abf4e79dbe73339b77778233a6c7d7f49f6b7d5db6a4885ff33585e221f5e94e8f7cc84ddcbe9c61a3d40c4f503a4ec7e91edca5745454588eebb4f0dc4d251c0d88eb5fae5d5b651d16e56ef830f412cb7fccf643de4963b66852d3a775489b5abb394b6fa325c3dbb4a55dd06d44c5fc911f1305e55accf0dc0eb172788f5400aab3c867cc6c5ddb7cd3e57bb78a739416985a276825171f5a19750dede055aa3e5fca9b11e3606beae97d68e593631a2efd88cdeb9f43b5ac1d1d9f0164f0fb022ea44a4a48061629c83d8f5bc594e3655ee684102fe706d1e96178bb805105fe1c5326c951401a6e7c9a0b8b572e7b74c3fb25e8700a2e0e70b4621ae3878805397ea1b873ea5218fdaa4fc5d11cdf7ea3579601eca3750fa347edc08569b1f51606d35920253f85f33e6a757a585adf079173161af919f7ea0d78ca6ca1513d01855057373c4f9fe22aba1fc4b18708d329500c127b865a528435e9e00d0a80554ae6eaf4d58bf85a959f37d0854b36c782991c36120b41ee2d9905b18d525b6bffef310e90dbfbe9be853614e6559737f1141f725902f59ee02789c6490c16adf0957e36dc4101c57ba35acb4ca9ec60f5585b60e74342921bbc7e56df5ad942b6deb7936532439b1dae39b9709cf282239c57b434d6f65ba277012ccddce32a217964f974c16f96d8b078ceaad43de9f3d5309279843f2f347ad8ae6eab3a998bb99a421b22b806e2f2302f9dcf3ba54e3d3f1ee64ef3b202194912eec202c2f44847ad5293b03b6b22df35f505670a79219efc399c6a4fa3fd4be7953e5df9baf94101c0a7036b82b6950ab2b722e38aec47bf1c7ffb4e82f43b9ca18d2a8b0b2a7b92015b01d07a429d2660902185cf143f871ff49dde73acf7c3bfd9c124733bd90ffe0fd1cc9090d56dd70bd62f9df1bfa4748ea3438f669d5691c61ec7fbc9d53ab4d8c2dda2cf203f7a5a7fac72eb2efe1d9a27b8c5b14e07a55c530dfd7b7c69dcf478590b7b364f5379f92a0762be0005c4cbc5285d7828248159286fe6d29c02c7de04e96e737a2d30ce75ff774982433f75ca16f09ad668e5b13f0a2e84886773d8fff67f71c1a9dab13f78e5b2da9b1eed9ab2208934a6da7eab32b3e8da1599d6cfa7e9c19ad8efc85dd9a2a4b95832c435381c2fe7e44c58045ce91e40d58c36924b38b19cbafd696bac8761229de9099ce31ee1c93a98aa0cb2a7c60b71b7f1998690e5eae623827727cfe7e8eed94ffc927a1e15aac32292daccda4f0d35383ce87f7e872fc3fe8f01f4a44de4f7b76257abc9c056ab8ae0d96d2dc3a154408c28a2e7befbd515cb5013cbfed31af456ac2b596b5d8095420c411b981d48741dc7ed1e8de4e428bd5e5a553348e2890b1ed12b7dc88261ab921a12da43e6344bbb4a0e0ce2b84c2d1d6c1f51b88202743433ac24340ae00cf27d43346240f4dc5e35ec29fcf1bf6de3bcc09ee8db3f49c3b6615bd8796bbe2cf4b914766779408e772123d9e51cc92ed5dedafa427fd767198cb97674eded4e4df84716aec75cbe7a54620c283fa60780be3cd66ea4167f46cdea1506be92a5102317c8ab8be097c993d82bd831818fe7cb1fbfecc3432d93e0f6d36da8a65ed15c78e623d59980be7ff54bdb1786de2ca9e7a11f0fe067db9ec42ade3bbaad10adae5ea77ba76fa2d0723a35891bde91da540a58e343c23afa9e22b38a66171eb9dbbd55f9e0f014e9de3943388fe0990cc801bbb978c02bf680b3c63a747e22a6317440c40e6844987e936c88c25f49e601ec3486ab080165b5e01dbee47a0a385dfba22ec5ed075f94052bdddabde761bbcc79852402c5b22ded89af4c602922099e37d71b7f87f4ffa614b4ca106fca6b062cba350be1fd12c6812db82f3e02a81e42*1*64*bbc3babf62557aa4dfba705e24274e1aebf43907fe12f52eaf5395066f7cbdba </td>
	</tr>
	<tr class="row193">
		<td class="col0"> 13400 </td><td class="col1"> Keepass 2 AES / with keyfile </td><td class="col2"> $keepass$*2*6000*222*15b6b685bae998f2f608c909dc554e514f2843fbac3c7c16ea3600cc0de30212*c417098b445cfc7a87d56ba17200836f30208d38f75a4169c0280bab3b10ca2a*0d15a81eadccc58b1d3942090cd0ba66*57c4aa5ac7295a97da10f8b2f2d2bfd7a98b0faf75396bc1b55164a1e1dc7e52*2b822bb7e7d060bb42324459cb24df4d3ecd66dc5fc627ac50bf2d7c4255e4f8*1*64*aaf72933951a03351e032b382232bcafbeeabc9bc8e6988b18407bc5b8f0e3cc </td>
	</tr>
	<tr class="row194">
		<td class="col0"> 13500 </td><td class="col1"> PeopleSoft PS_TOKEN </td><td class="col2"> b5e335754127b25ba6f99a94c738e24cd634c35a:aa07d396f5038a6cbeded88d78d1d6c907e4079b3dc2e12fddee409a51cc05ae73e8cc24d518c923a2f79e49376594503e6238b806bfe33fa8516f4903a9b4 </td>
	</tr>
	<tr class="row195">
		<td class="col0"> 13600 </td><td class="col1"> WinZip </td><td class="col2"> $zip2$*0*3*0*e3222d3b65b5a2785b192d31e39ff9de*1320*e*19648c3e063c82a9ad3ef08ed833*3135c79ecb86cd6f48fc*$/zip2$ </td>
	</tr>
	<tr class="row196">
		<td class="col0"> 13711 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_13711.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_13711.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_13711.vc</a> </td>
	</tr>
	<tr class="row197">
		<td class="col0"> 13712 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_13712.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_13712.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_13712.vc</a> </td>
	</tr>
	<tr class="row198">
		<td class="col0"> 13711 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent_13711.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent_13711.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent_13711.vc</a> </td>
	</tr>
	<tr class="row199">
		<td class="col0"> 13712 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-aes_13712.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-aes_13712.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-aes_13712.vc</a> </td>
	</tr>
	<tr class="row200">
		<td class="col0"> 13713 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-twofish-aes_13713.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-twofish-aes_13713.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_serpent-twofish-aes_13713.vc</a> </td>
	</tr>
	<tr class="row201">
		<td class="col0"> 13711 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish_13711.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish_13711.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish_13711.vc</a> </td>
	</tr>
	<tr class="row202">
		<td class="col0"> 13712 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish-serpent_13712.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish-serpent_13712.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_twofish-serpent_13712.vc</a> </td>
	</tr>
	<tr class="row203">
		<td class="col0"> 13751 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_13751.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_13751.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_13751.vc</a> </td>
	</tr>
	<tr class="row204">
		<td class="col0"> 13752 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes-twofish_13752.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes-twofish_13752.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes-twofish_13752.vc</a> </td>
	</tr>
	<tr class="row205">
		<td class="col0"> 13751 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent_13751.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent_13751.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent_13751.vc</a> </td>
	</tr>
	<tr class="row206">
		<td class="col0"> 13752 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_13752.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_13752.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_13752.vc</a> </td>
	</tr>
	<tr class="row207">
		<td class="col0"> 13753 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_13753.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_13753.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_13753.vc</a> </td>
	</tr>
	<tr class="row208">
		<td class="col0"> 13751 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_13751.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_13751.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_13751.vc</a> </td>
	</tr>
	<tr class="row209">
		<td class="col0"> 13752 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish-serpent_13752.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish-serpent_13752.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish-serpent_13752.vc</a> </td>
	</tr>
	<tr class="row210">
		<td class="col0"> 13721 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes_13721.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes_13721.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes_13721.vc</a> </td>
	</tr>
	<tr class="row211">
		<td class="col0"> 13722 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes-twofish_13722.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes-twofish_13722.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_aes-twofish_13722.vc</a> </td>
	</tr>
	<tr class="row212">
		<td class="col0"> 13721 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent_13721.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent_13721.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent_13721.vc</a> </td>
	</tr>
	<tr class="row213">
		<td class="col0"> 13722 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-aes_13722.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-aes_13722.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-aes_13722.vc</a> </td>
	</tr>
	<tr class="row214">
		<td class="col0"> 13723 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-twofish-aes_13723.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-twofish-aes_13723.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_serpent-twofish-aes_13723.vc</a> </td>
	</tr>
	<tr class="row215">
		<td class="col0"> 13721 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish_13721.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish_13721.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish_13721.vc</a> </td>
	</tr>
	<tr class="row216">
		<td class="col0"> 13722 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA512 + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish-serpent_13722.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish-serpent_13722.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha512_twofish-serpent_13722.vc</a> </td>
	</tr>
	<tr class="row217">
		<td class="col0"> 13731 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes_13731.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes_13731.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes_13731.vc</a> </td>
	</tr>
	<tr class="row218">
		<td class="col0"> 13732 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes-twofish_13732.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes-twofish_13732.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_aes-twofish_13732.vc</a> </td>
	</tr>
	<tr class="row219">
		<td class="col0"> 13731 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent_13731.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent_13731.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent_13731.vc</a> </td>
	</tr>
	<tr class="row220">
		<td class="col0"> 13732 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-aes_13732.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-aes_13732.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-aes_13732.vc</a> </td>
	</tr>
	<tr class="row221">
		<td class="col0"> 13733 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-twofish-aes_13733.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-twofish-aes_13733.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_serpent-twofish-aes_13733.vc</a> </td>
	</tr>
	<tr class="row222">
		<td class="col0"> 13731 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish_13731.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish_13731.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish_13731.vc</a> </td>
	</tr>
	<tr class="row223">
		<td class="col0"> 13732 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-Whirlpool + Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish-serpent_13732.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish-serpent_13732.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_whirlpool_twofish-serpent_13732.vc</a> </td>
	</tr>
	<tr class="row224">
		<td class="col0"> 13741 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + boot-mode + AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes_boot.vc</a> </td>
	</tr>
	<tr class="row225">
		<td class="col0"> 13742 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + boot-mode + AES-Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish_boot.vc</a> </td>
	</tr>
	<tr class="row226">
		<td class="col0"> 13743 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-RIPEMD160 + boot-mode + AES-Twofish-Serpent </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish-serpent_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish-serpent_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_ripemd160_aes-twofish-serpent_boot.vc</a> </td>
	</tr>
	<tr class="row227">
		<td class="col0"> 13761 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + boot-mode + Twofish </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_twofish_boot.vc</a> </td>
	</tr>
	<tr class="row228">
		<td class="col0"> 13762 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + boot-mode + Serpent-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-aes_boot.vc</a> </td>
	</tr>
	<tr class="row229">
		<td class="col0"> 13763 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + boot-mode + Serpent-Twofish-AES </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_boot.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_boot.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_serpent-twofish-aes_boot.vc</a> </td>
	</tr>
	<tr class="row230">
		<td class="col0"> 13761 </td><td class="col1"> VeraCrypt PBKDF2-HMAC-SHA256 + boot-mode + PIM + AES <sup>16</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_boot_pim500.vc" class="urlextern" title="https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_boot_pim500.vc" rel="nofollow">https://hashcat.net/misc/example_hashes/vc/hashcat_sha256_aes_boot_pim500.vc</a> </td>
	</tr>
	<tr class="row231">
		<td class="col0"> 13771 </td><td class="col1"> VeraCrypt Streebog-512 + XTS 512 bit </td><td class="col2"> TBD </td>
	</tr>
	<tr class="row232">
		<td class="col0"> 13772 </td><td class="col1"> VeraCrypt Streebog-512 + XTS 1024 bit </td><td class="col2"> TBD </td>
	</tr>
	<tr class="row233">
		<td class="col0"> 13773 </td><td class="col1"> VeraCrypt Streebog-512 + XTS 1536 bit </td><td class="col2"> TBD </td>
	</tr>
	<tr class="row234">
		<td class="col0"> 13800 </td><td class="col1"> Windows Phone 8+ PIN/password </td><td class="col2"> 95fc4680bcd2a5f25de3c580cbebadbbf256c1f0ff2e9329c58e36f8b914c11f:4471347156480581513210137061422464818088437334031753080747625028271635402815635172140161077854162657165115624364524648202480341513407048222056541500234214433548175101668212658151115765112202168288664210443352443335235337677853484573107775345675846323265745 </td>
	</tr>
	<tr class="row235">
		<td class="col0"> 13900 </td><td class="col1"> OpenCart </td><td class="col2"> 6e36dcfc6151272c797165fce21e68e7c7737e40:472433673 </td>
	</tr>
	<tr class="row236">
		<td class="col0"> 14000 </td><td class="col1"> DES (PT = $salt, key = $pass) <sup>8</sup> </td><td class="col2"> a28bc61d44bb815c:1172075784504605 </td>
	</tr>
	<tr class="row237">
		<td class="col0"> 14100 </td><td class="col1"> 3DES (PT = $salt, key = $pass) <sup>9</sup> </td><td class="col2"> 37387ff8d8dafe15:8152001061460743 </td>
	</tr>
	<tr class="row238">
		<td class="col0"> 14400 </td><td class="col1"> sha1(CX) </td><td class="col2"> fd9149fb3ae37085dc6ed1314449f449fbf77aba:87740665218240877702 </td>
	</tr>
	<tr class="row239">
		<td class="col0"> 14600 </td><td class="col1"> LUKS <sup>10</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/hashcat_luks_testfiles.7z" class="urlextern" title="https://hashcat.net/misc/example_hashes/hashcat_luks_testfiles.7z" rel="nofollow">https://hashcat.net/misc/example_hashes/hashcat_luks_testfiles.7z</a> </td>
	</tr>
	<tr class="row240">
		<td class="col0"> 14700 </td><td class="col1"> iTunes backup &lt; 10.0 <sup>11</sup> </td><td class="col2"> $itunes_backup$*9*b8e3f3a970239b22ac199b622293fe4237b9d16e74bad2c3c3568cd1bd3c471615a6c4f867265642*10000*4542263740587424862267232255853830404566** </td>
	</tr>
	<tr class="row241">
		<td class="col0"> 14800 </td><td class="col1"> iTunes backup &gt;= 10.0 <sup>11</sup> </td><td class="col2"> $itunes_backup$*10*8b715f516ff8e64442c478c2d9abb046fc6979ab079007d3dbcef3ddd84217f4c3db01362d88fa68*10000*2353363784073608264337337723324886300850*10000000*425b4bb4e200b5fd4c66979c9caca31716052063 </td>
	</tr>
	<tr class="row242">
		<td class="col0"> 14900 </td><td class="col1"> Skip32 (PT = $salt, key = $pass) <sup>12</sup> </td><td class="col2"> c9350366:44630464 </td>
	</tr>
	<tr class="row243">
		<td class="col0"> 15000 </td><td class="col1"> FileZilla Server &gt;= 0.9.55 </td><td class="col2"> 632c4952b8d9adb2c0076c13b57f0c934c80bdc14fc1b4c341c2e0a8fd97c4528729c7bd7ed1268016fc44c3c222445ebb880eca9a6638ea5df74696883a2978:0608516311148050266404072407085605002866301131581532805665756363 </td>
	</tr>
	<tr class="row244">
		<td class="col0"> 15100 </td><td class="col1"> Juniper/NetBSD sha1crypt </td><td class="col2"> $sha1$15100$jiJDkz0E$E8C7RQAD3NetbSDz7puNAY.5Y2jr </td>
	</tr>
	<tr class="row245">
		<td class="col0"> 15200 </td><td class="col1"> Blockchain, My Wallet, V2 </td><td class="col2"> $blockchain$v2$5000$288$06063152445005516247820607861028813ccf6dcc5793dc0c7a82dcd604c5c3e8d91bea9531e628c2027c56328380c87356f86ae88968f179c366da9f0f11b09492cea4f4d591493a06b2ba9647faee437c2f2c0caaec9ec795026af51bfa68fc713eaac522431da8045cc6199695556fc2918ceaaabbe096f48876f81ddbbc20bec9209c6c7bc06f24097a0e9a656047ea0f90a2a2f28adfb349a9cd13852a452741e2a607dae0733851a19a670513bcf8f2070f30b115f8bcb56be2625e15139f2a357cf49d72b1c81c18b24c7485ad8af1e1a8db0dc04d906935d7475e1d3757aba32428fdc135fee63f40b16a5ea701766026066fb9fb17166a53aa2b1b5c10b65bfe685dce6962442ece2b526890bcecdeadffbac95c3e3ad32ba57c9e </td>
	</tr>
	<tr class="row246">
		<td class="col0"> 15300 </td><td class="col1"> DPAPI master key file version 1 + local context </td><td class="col2"> $DPAPImk$1*1*S-15-21-466364039-425773974-453930460-1925*des3*sha1*24000*b038489dee5ad04e3e3cab4d957258b5*208*cb9b5b7d96a0d2a00305ca403d3fd9c47c561e35b4b2cf3aebfd1d3199a6481d56972be7ebd6c291b199e6f1c2ffaee91978706737e9b1209e6c7d3aa3d8c3c3e38ad1ccfa39400d62c2415961c17fd0bd6b0f7bbd49cc1de1a394e64b7237f56244238da8d37d78 </td>
	</tr>
	<tr class="row247">
		<td class="col0"> 15400 </td><td class="col1"> ChaCha20 </td><td class="col2"> $chacha20$*0400000000000003*9*0200000000000001*4a4b4c4d4e4f5051*676e31b5ad612c2b </td>
	</tr>
	<tr class="row248">
		<td class="col0"> 15500 </td><td class="col1"> JKS Java Key Store Private Keys (SHA1) </td><td class="col2"> $jksprivk$*5A3AA3C3B7DD7571727E1725FB09953EF3BEDBD9*0867403720562514024857047678064085141322*81*C3*50DDD9F532430367905C9DE31FB1*test </td>
	</tr>
	<tr class="row249">
		<td class="col0"> 15600 </td><td class="col1"> Ethereum Wallet, PBKDF2-HMAC-SHA256 </td><td class="col2"> $ethereum$p*262144*3238383137313130353438343737383736323437353437383831373034343735*06eae7ee0a4b9e8abc02c9990e3730827396e8531558ed15bb733faf12a44ce1*e6d5891d4f199d31ec434fe25d9ecc2530716bc3b36d5bdbc1fab7685dda3946 </td>
	</tr>
	<tr class="row250">
		<td class="col0"> 15700 </td><td class="col1"> Ethereum Wallet, SCRYPT </td><td class="col2"> $ethereum$s*262144*1*8*3436383737333838313035343736303637353530323430373235343034363130*8b58d9d15f579faba1cd13dd372faeb51718e7f70735de96f0bcb2ef4fb90278*8de566b919e6825a65746e266226316c1add8d8c3d15f54640902437bcffc8c3 </td>
	</tr>
	<tr class="row251">
		<td class="col0"> 15900 </td><td class="col1"> DPAPI master key file version 2 + Active Directory domain context </td><td class="col2"> $DPAPImk$2*2*S-15-21-423929668-478423897-489523715-1834*aes256*sha512*8000*740866e4105c77f800f02d367dd96699*288*ebc2907e16245dfe6c902ad4be70a079e62204c8a947498455056d150e6babb3c90b1616a8dff0e390dd26dda1978dffcbd7b9d7d1ea5c6d3e4df36db4d977051ec01fd6f0882a597c51834cb86445cad50c716f48b37cfd24339d8b43da771526fb01376798251edaa868fa2b1fa85c4142864b899987d4bbdc87b53433ed945fa4ab49c7f9d4d01df3ae19f25013b2 </td>
	</tr>
	<tr class="row252">
		<td class="col0"> 16000 </td><td class="col1"> Tripcode </td><td class="col2"> pfaRCwDe0U </td>
	</tr>
	<tr class="row253">
		<td class="col0"> 16100 </td><td class="col1"> TACACS+ </td><td class="col2"> $tacacs-plus$0$5fde8e68$4e13e8fb33df$c006 </td>
	</tr>
	<tr class="row254">
		<td class="col0"> 16200 </td><td class="col1"> Apple Secure Notes </td><td class="col2"> $ASN$*1*20000*80771171105233481004850004085037*d04b17af7f6b184346aad3efefe8bec0987ee73418291a41 </td>
	</tr>
	<tr class="row255">
		<td class="col0"> 16300 </td><td class="col1"> Ethereum Pre-Sale Wallet, PBKDF2-HMAC-SHA256 </td><td class="col2"> $ethereum$w*e94a8e49deac2d62206bf9bfb7d2aaea7eb06c1a378cfc1ac056cc599a569793c0ecc40e6a0c242dee2812f06b644d70f43331b1fa2ce4bd6cbb9f62dd25b443235bdb4c1ffb222084c9ded8c719624b338f17e0fd827b34d79801298ac75f74ed97ae16f72fccecf862d09a03498b1b8bd1d984fc43dd507ede5d4b6223a582352386407266b66c671077eefc1e07b5f42508bf926ab5616658c984968d8eec25c9d5197a4a30eed54c161595c3b4d558b17ab8a75ccca72b3d949919d197158ea5cfbc43ac7dd73cf77807dc2c8fe4ef1e942ccd11ec24fe8a410d48ef4b8a35c93ecf1a21c51a51a08f3225fbdcc338b1e7fdafd7d94b82a81d88c2e9a429acc3f8a5974eafb7af8c912597eb6fdcd80578bd12efddd99de47b44e7c8f6c38f2af3116b08796172eda89422e9ea9b99c7f98a7e331aeb4bb1b06f611e95082b629332c31dbcfd878aed77d300c9ed5c74af9cd6f5a8c4a261dd124317fb790a04481d93aec160af4ad8ec84c04d943a869f65f07f5ccf8295dc1c876f30408eac77f62192cbb25842470b4a5bdb4c8096f56da7e9ed05c21f61b94c54ef1c2e9e417cce627521a40a99e357dd9b7a7149041d589cbacbe0302db57ddc983b9a6d79ce3f2e9ae8ad45fa40b934ed6b36379b780549ae7553dbb1cab238138c05743d0103335325bd90e27d8ae1ea219eb8905503c5ad54fa12d22e9a7d296eee07c8a7b5041b8d56b8af290274d01eb0e4ad174eb26b23b5e9fb46ff7f88398e6266052292acb36554ccb9c2c03139fe72d3f5d30bd5d10bd79d7cb48d2ab24187d8efc3750d5a24980fb12122591455d14e75421a2074599f1cc9fdfc8f498c92ad8b904d3c4307f80c46921d8128*f3abede76ac15228f1b161dd9660bb9094e81b1b*d201ccd492c284484c7824c4d37b1593 </td>
	</tr>
	<tr class="row256">
		<td class="col0"> 16400 </td><td class="col1"> CRAM-MD5 Dovecot </td><td class="col2"> {CRAM-MD5}5389b33b9725e5657cb631dc50017ff1535ce4e2a1c414009126506fc4327d0d </td>
	</tr>
	<tr class="row257">
		<td class="col0"> 16500 </td><td class="col1"> JWT (JSON Web Token) </td><td class="col2"> eyJhbGciOiJIUzI1NiJ9.eyIzNDM2MzQyMCI6NTc2ODc1NDd9.f1nXZ3V_Hrr6ee-AFCTLaHRnrkiKmio2t3JqwL32guY </td>
	</tr>
	<tr class="row258">
		<td class="col0"> 16600 </td><td class="col1"> Electrum Wallet (Salt-Type 1-3) </td><td class="col2"> $electrum$1*44358283104603165383613672586868*c43a6632d9f59364f74c395a03d8c2ea </td>
	</tr>
	<tr class="row259">
		<td class="col0"> 16700 </td><td class="col1"> FileVault 2 </td><td class="col2"> $fvde$1$16$84286044060108438487434858307513$20000$f1620ab93192112f0a23eea89b5d4df065661f974b704191 </td>
	</tr>
	<tr class="row260">
		<td class="col0"> 16800 </td><td class="col1"> WPA-PMKID-PBKDF2 <sup>1</sup> </td><td class="col2"> 2582a8281bf9d4308d6f5731d0e61c61*4604ba734d4e*89acf0e761f4*ed487162465a774bfba60eb603a39f3a </td>
	</tr>
	<tr class="row261">
		<td class="col0"> 16801 </td><td class="col1"> WPA-PMKID-PMK <sup>15</sup> </td><td class="col2"> 2582a8281bf9d4308d6f5731d0e61c61*4604ba734d4e*89acf0e761f4 </td>
	</tr>
	<tr class="row262">
		<td class="col0"> 16900 </td><td class="col1"> Ansible Vault </td><td class="col2"> $ansible$0*0*6b761adc6faeb0cc0bf197d3d4a4a7d3f1682e4b169cae8fa6b459b3214ed41e*426d313c5809d4a80a4b9bc7d4823070*d8bad190c7fbc7c3cb1c60a27abfb0ff59d6fb73178681c7454d94a0f56a4360 </td>
	</tr>
	<tr class="row263">
		<td class="col0"> 17200 </td><td class="col1"> PKZIP (Compressed) <sup>*</sup> </td><td class="col2"> $pkzip2$1*1*2*0*e3*1c5*eda7a8de*0*28*8*e3*eda7*5096*a9fc1f4e951c8fb3031a6f903e5f4e3211c8fdc4671547bf77f6f682afbfcc7475d83898985621a7af9bccd1349d1976500a68c48f630b7f22d7a0955524d768e34868880461335417ddd149c65a917c0eb0a4bf7224e24a1e04cf4ace5eef52205f4452e66ded937db9545f843a68b1e84a2e933cc05fb36d3db90e6c5faf1bee2249fdd06a7307849902a8bb24ec7e8a0886a4544ca47979a9dfeefe034bdfc5bd593904cfe9a5309dd199d337d3183f307c2cb39622549a5b9b8b485b7949a4803f63f67ca427a0640ad3793a519b2476c52198488e3e2e04cac202d624fb7d13c2*$/pkzip2$ </td>
	</tr>
	<tr class="row264">
		<td class="col0"> 17210 </td><td class="col1"> PKZIP (Uncompressed) <sup>*</sup> </td><td class="col2"> $pkzip2$1*1*2*0*1d1*1c5*eda7a8de*0*28*0*1d1*eda7*5096*1dea673da43d9fc7e2be1a1f4f664269fceb6cb88723a97408ae1fe07f774d31d1442ea8485081e63f919851ca0b7588d5e3442317fff19fe547a4ef97492ed75417c427eea3c4e146e16c100a2f8b6abd7e5988dc967e5a0e51f641401605d673630ea52ebb04da4b388489901656532c9aa474ca090dbac7cf8a21428d57b42a71da5f3d83fed927361e5d385ca8e480a6d42dea5b4bf497d3a24e79fc7be37c8d1721238cbe9e1ea3ae1eb91fc02aabdf33070d718d5105b70b3d7f3d2c28b3edd822e89a5abc0c8fee117c7fbfbfd4b4c8e130977b75cb0b1da080bfe1c0859e6483c42f459c8069d45a76220e046e6c2a2417392fd87e4aa4a2559eaab3baf78a77a1b94d8c8af16a977b4bb45e3da211838ad044f209428dba82666bf3d54d4eed82c64a9b3444a44746b9e398d0516a2596d84243b4a1d7e87d9843f38e45b6be67fd980107f3ad7b8453d87300e6c51ac9f5e3f6c3b702654440c543b1d808b62f7a313a83b31a6faaeedc2620de7057cd0df80f70346fe2d4dccc318f0b5ed128bcf0643e63d754bb05f53afb2b0fa90b34b538b2ad3648209dff587df4fa18698e4fa6d858ad44aa55d2bba3b08dfdedd3e28b8b7caf394d5d9d95e452c2ab1c836b9d74538c2f0d24b9b577*$/pkzip2$ </td>
	</tr>
	<tr class="row265">
		<td class="col0"> 17220 </td><td class="col1"> PKZIP (Compressed Multi-File) <sup>*</sup> </td><td class="col2"> $pkzip2$3*1*1*0*8*24*a425*8827*d1730095cd829e245df04ebba6c52c0573d49d3bbeab6cb385b7fa8a28dcccd3098bfdd7*1*0*8*24*2a74*882a*51281ac874a60baedc375ca645888d29780e20d4076edd1e7154a99bde982152a736311f*2*0*e3*1c5*eda7a8de*0*29*8*e3*eda7*5096*1455781b59707f5151139e018bdcfeebfc89bc37e372883a7ec0670a5eafc622feb338f9b021b6601a674094898a91beac70e41e675f77702834ca6156111a1bf7361bc9f3715d77dfcdd626634c68354c6f2e5e0a7b1e1ce84a44e632d0f6e36019feeab92fb7eac9dda8df436e287aafece95d042059a1b27d533c5eab62c1c559af220dc432f2eb1a38a70f29e8f3cb5a207704274d1e305d7402180fd47e026522792f5113c52a116d5bb25b67074ffd6f4926b221555234aabddc69775335d592d5c7d22462b75de1259e8342a9ba71cb06223d13c7f51f13be2ad76352c3b8ed*$/pkzip2$ </td>
	</tr>
	<tr class="row266">
		<td class="col0"> 17225 </td><td class="col1"> PKZIP (Mixed Multi-File) <sup>*</sup> </td><td class="col2"> $pkzip2$3*1*1*0*0*24*3e2c*3ef8*0619e9d17ff3f994065b99b1fa8aef41c056edf9fa4540919c109742dcb32f797fc90ce0*1*0*8*24*431a*3f26*18e2461c0dbad89bd9cc763067a020c89b5e16195b1ac5fa7fb13bd246d000b6833a2988*2*0*23*17*1e3c1a16*2e4*2f*0*23*1e3c*3f2d*54ea4dbc711026561485bbd191bf300ae24fa0997f3779b688cdad323985f8d3bb8b0c*$/pkzip2$ </td>
	</tr>
	<tr class="row267">
		<td class="col0"> 17230 </td><td class="col1"> PKZIP (Compressed Multi-File Checksum-Only) <sup>*</sup> </td><td class="col2"> $pkzip2$8*1*1*0*8*24*a425*8827*3bd479d541019c2f32395046b8fbca7e1dca218b9b5414975be49942c3536298e9cc939e*1*0*8*24*2a74*882a*537af57c30fd9fd4b3eefa9ce55b6bff3bbfada237a7c1dace8ebf3bb0de107426211da3*1*0*8*24*2a74*882a*5f406b4858d3489fd4a6a6788798ac9b924b5d0ca8b8e5a6371739c9edcfd28c82f75316*1*0*8*24*2a74*882a*1843aca546b2ea68bd844d1e99d4f74d86417248eb48dd5e956270e42a331c18ea13f5ed*1*0*8*24*2a74*882a*aca3d16543bbfb2e5d2659f63802e0fa5b33e0a1f8ae47334019b4f0b6045d3d8eda3af1*1*0*8*24*2a74*882a*fbe0efc9e10ae1fc9b169bd060470bf3e39f09f8d83bebecd5216de02b81e35fe7e7b2f2*1*0*8*24*2a74*882a*537886dbabffbb7cac77deb01dc84760894524e6966183b4478a4ef56f0c657375a235a1*1*0*8*24*eda7*5096*40eb30ef1ddd9b77b894ed46abf199b480f1e5614fde510855f92ae7b8026a11f80e4d5f*$/pkzip2$ </td>
	</tr>
	<tr class="row268">
		<td class="col0"> 17300 </td><td class="col1"> SHA3-224 </td><td class="col2"> 412ef78534ba6ab0e9b1607d3e9767a25c1ea9d5e83176b4c2817a6c </td>
	</tr>
	<tr class="row269">
		<td class="col0"> 17400 </td><td class="col1"> SHA3-256 </td><td class="col2"> d60fcf6585da4e17224f58858970f0ed5ab042c3916b76b0b828e62eaf636cbd </td>
	</tr>
	<tr class="row270">
		<td class="col0"> 17500 </td><td class="col1"> SHA3-384 </td><td class="col2"> 983ba28532cc6320d04f20fa485bcedb38bddb666eca5f1e5aa279ff1c6244fe5f83cf4bbf05b95ff378dd2353617221 </td>
	</tr>
	<tr class="row271">
		<td class="col0"> 17600 </td><td class="col1"> SHA3-512 </td><td class="col2"> 7c2dc1d743735d4e069f3bda85b1b7e9172033dfdd8cd599ca094ef8570f3930c3f2c0b7afc8d6152ce4eaad6057a2ff22e71934b3a3dd0fb55a7fc84a53144e </td>
	</tr>
	<tr class="row272">
		<td class="col0"> 17700 </td><td class="col1"> Keccak-224 </td><td class="col2"> e1dfad9bafeae6ef15f5bbb16cf4c26f09f5f1e7870581962fc84636 </td>
	</tr>
	<tr class="row273">
		<td class="col0"> 17800 </td><td class="col1"> Keccak-256 </td><td class="col2"> 203f88777f18bb4ee1226627b547808f38d90d3e106262b5de9ca943b57137b6 </td>
	</tr>
	<tr class="row274">
		<td class="col0"> 17900 </td><td class="col1"> Keccak-384 </td><td class="col2"> 5804b7ada5806ba79540100e9a7ef493654ff2a21d94d4f2ce4bf69abda5d94bf03701fe9525a15dfdc625bfbd769701 </td>
	</tr>
	<tr class="row275">
		<td class="col0"> 18000 </td><td class="col1"> Keccak-512 </td><td class="col2"> 2fbf5c9080f0a704de2e915ba8fdae6ab00bbc026b2c1c8fa07da1239381c6b7f4dfd399bf9652500da723694a4c719587dd0219cb30eabe61210a8ae4dc0b03 </td>
	</tr>
	<tr class="row276">
		<td class="col0"> 18100 </td><td class="col1"> TOTP (HMAC-SHA1) </td><td class="col2"> 597056:3600 </td>
	</tr>
	<tr class="row277">
		<td class="col0"> 18200 </td><td class="col1"> Kerberos 5 AS-REP etype 23 </td><td class="col2"> $krb5asrep$23$user@domain.com:3e156ada591263b8aab0965f5aebd837$007497cb51b6c8116d6407a782ea0e1c5402b17db7afa6b05a6d30ed164a9933c754d720e279c6c573679bd27128fe77e5fea1f72334c1193c8ff0b370fadc6368bf2d49bbfdba4c5dccab95e8c8ebfdc75f438a0797dbfb2f8a1a5f4c423f9bfc1fea483342a11bd56a216f4d5158ccc4b224b52894fadfba3957dfe4b6b8f5f9f9fe422811a314768673e0c924340b8ccb84775ce9defaa3baa0910b676ad0036d13032b0dd94e3b13903cc738a7b6d00b0b3c210d1f972a6c7cae9bd3c959acf7565be528fc179118f28c679f6deeee1456f0781eb8154e18e49cb27b64bf74cd7112a0ebae2102ac </td>
	</tr>
	<tr class="row278">
		<td class="col0"> 18300 </td><td class="col1"> Apple File System (APFS) </td><td class="col2"> $fvde$2$16$58778104701476542047675521040224$20000$39602e86b7cea4a34f4ff69ff6ed706d68954ee474de1d2a9f6a6f2d24d172001e484c1d4eaa237d </td>
	</tr>
	<tr class="row279">
		<td class="col0"> 18400 </td><td class="col1"> Open Document Format (ODF) 1.2 (SHA-256, AES) <sup>*</sup> </td><td class="col2"> $odf$*1*1*100000*32*751854d8b90731ce0579f96bea6f0d4ac2fb2f546b31f1b6af9a5f66952a0bf4*16*2185a966155baa9e2fb597298febecbc*16*c18eaae34bcbbe9119be017fe5f8b52d*0*051e0f1ce0e866f2b771029e03a6c7119aad132af54c4e45824f16f61f357a40407ab82744fe6370c7b2346075fcd4c2e58ab244411b3ab1d532a46e2321599ef13c3d3472fc2f14d480d8c33215e473da67f90540279d3ef1f62dde314fa222796046e496c951235ddf88aa754620b7810d22ebc8835c90dce9276946f52b8ea7d95d2f86e4cc725366a8b3edacc2ce88518e535991a5f84d5ea8795dc02bfb731b5f202ecaf7d4b245d928c4248709fcdf3fba2acf1a08be0c1eee7dbeda07e8c3a6983565635e99952b8ad79d31c965f245ae90b5cc3dba6387898c66fa35cad9ac9595c41b62e68efcdd73185b38e220cf004269b77ec6974474b03b7569afc3b503a2bf8b2d035756f3f4cb880d9ba815e5c944508a0bde214076c35bf0e0814a96d21ccaa744c9056948ed935209f5c7933841d2ede3d28dd84da89d477d4a0041ce6d8ddab891d929340db6daa921d69b46fd5aee306d0bcef88c38acbb495d0466df7e2f744e3d10201081215c02db5dd479a4cda15a3338969c7baec9d3d2c378a8dd30449319b149dc3b4e7f00996a59fcb5f243d0df2cbaf749241033f7865aefa960adfeb8ebf205b270f90b1f82c34f80d5a8a0db7aec89972a32f5daa2a73c5895d1fced01b3ab8e576bd2630eff01cad97781f4966d4b528e1b15f011f28ae907a352073c96b203adc7742d2b79b2e2f440b17e7856ae119e08d15d8bdf951f6d4a3f9b516da2d9a8f9dd93488f8e0119f3da19138ab787f0d7098a652cccd914aa0ff81d375bd6a5a165acc936f591639059287975cfc3ca4342e5f9501b3249a76d14e56d6d56b319e036bc0449ac7b5afa24ffbea11babed8183edf8d4fdca1c3f0d23bfd4a02797627d556634f1a9304e03737604bd86f6b5a26aa687d6df73383e0f7dfe62a131e8dbb8c3f4f13d24857dd29d76984eac6c45df7428fc79323ffa1f4e7962d705df74320141ed1f16d1ad483b872168df60315ffadbfa1b7f4afaed8a0017421bf5e05348cb5c707a5e852d6fee6077ec1c33bc707bcd97b7701ee05a03d6fa78b0d31c8c97ea16e0edf434961bd5cc7cbb7eb2553730f0405c9bd21cee09b3f7c1bc57779fdfc15f3935985737a1b522004c4436b631a39a66e8577a03f5020e6aa41952c0662c8c57f66caa483b47af38b8cb5d457245fd3241749e17433e6f929233e8862d7c584111b1991b2d6e94278e7e6e1908cee5a83d94c78b75a84a695d25aeb9fdde72174fe6dd75e8d406671f44892a385a4a1e249f61ebc993e985607423a0a5742e668d52c1ebf5cecae7c2b7908f4627b92ec49354a9ccff8cb5763ad074a00e65a485a41bf4c25ce7e6fae49358a58547b1c0ca79713e297310c0a367c3de196f1dd685ca4be643bdf1e4f6b034211d020557e37a3b6614d061010b4a3416b6b279728c245d3322 </td>
	</tr>
	<tr class="row280">
		<td class="col0"> 18500 </td><td class="col1"> sha1(md5(md5($pass))) <sup>*</sup> </td><td class="col2"> 888a2ffcb3854fba0321110c5d0d434ad1aa2880 </td>
	</tr>
	<tr class="row281">
		<td class="col0"> 18600 </td><td class="col1"> Open Document Format (ODF) 1.1 (SHA-1, Blowfish) <sup>*</sup> </td><td class="col2"> $odf$*0*0*1024*16*bff753835f4ea15644b8a2f8e4b5be3d147b9576*8*ee371da34333b69d*16*a902eff54a4d782a26a899a31f97bef4*0*dae7e41fbc3a500d3ce152edd8876c4f38fb17d673ee2ac44ef1e0e283622cd2ae298a82d8d98f2ea737247881fc353e73a2f535c6e13e0cdc60821c1a61c53a4b0c46ff3a3b355d7b793fad50de15999fc7c1194321d1c54316c3806956c4a3ade7daabb912a2a36398eba883af088b3cb69b43365d9ba9fce3fb0c1524f73947a7e9fc1bf3adb5f85a367035feacb5d97c578b037144c2793f34aa09dcd04bdaa455aee0d4c52fe377248611dd56f2bd4eb294673525db905f5d905a28dec0909348e6bf94bcebf03ddd61a48797cd5728ce6dbb71037b268f526e806401abcf495f6edd0b5d87118671ec690d4627f86a43e51c7f6d42a75a56eec51204d47e115e813ed4425c97b16b195e02ce776c185194b9de43ae89f356e29face016cb393d6fb93af8ea305d921d5592dd184051ac790b9b90266f52b8d53ce1cb1d762942d6d5bbd0e3821be21af9fa6874ba0c60e64f41d3e5b6caca1c53b575afdc5d8f6a3edbf874dbe009c6cb296466fe9637aed4aed8a43a95ea7d26b4090ad33d4ee7a83844b0893e8bc0f04944205fb9576cb5720f019028cd75ca9ac47b3e5fa231354d74135564df43b659cfaea7e195c4a896e0e0e0c85dc9ce3a9ce9ba552bc2a6dbac4901c19558818e1957ed72d78662bb5ba53475ca584371f1825ae0c92322a4404e63c2baad92665aac29b5c6f96e1e6338d48fb0aef4d0b686063974f58b839484f8dcf0a02537cba67a7d2c4de13125d74820cb07ec72782035af1ea6c4db61c77016d1c021b63c8b07adb4e8510f5c41bbc501f60f3dd16462399b52eb146787e38e700147c7aa23ac4d5d22d9d1c93e67a01c92a197d4765cbf8d56a862a1205abb450a182913a69b8d5334a59924f86fb3ccd0dcfe7426053e26ba26b57c05f38d85863fff1f81135b0366e8cd8680663ae8aaf7d005317b849d5e08be882708fa0d8d02d47e89150124b507c34845c922b95e62aa0b3fef218773d7aeb572c67b35ad8787f31ecc6e1846b673b8ba6172223176eabf0020b6aa3aa71405b40b2fc2127bf9741a103f1d8eca21bf27328cdf15153f2f223eff7b831a72ed8ecacf4ea8df4ea44f3a3921e5a88fb2cfa355ece0f05cbc88fdd1ecd368d6e3b2dfabd999e5b708f1bccaeebb296c9d7b76659967742fe966aa6871cbbffe710b0cd838c6e02e6eb608cb5c81d066b60b5b3604396331d97d4a2c4c2317406e48c9f5387a2c72511d1e6899bd450e9ca88d535755bcfddb53a6df118cd9cdc7d8b4b814f7bc17684d8e5975defaa25d06f410ed0724c16b8f69ec3869bc1f05c71483666968d1c04509875dadd72c6182733d564eb1a7d555dc34f6b817c5418626214d0b2c3901c5a46f5b20fddfdf9f71a7dfd75b9928778a3f65e1832dff22be973c2b259744d500a3027c2a2e08972eaaad4c5c4ec871 </td>
	</tr>
	<tr class="row282">
		<td class="col0"> 18700 </td><td class="col1"> Java Object hashCode() <sup>*</sup> </td><td class="col2"> 29937c08 </td>
	</tr>
	<tr class="row283">
		<td class="col0"> 18800 </td><td class="col1"> Blockchain, My Wallet, Second Password (SHA256) <sup>*</sup> </td><td class="col2"> YnM6WYERjJfhxwepT7zV6odWoEUz1X4esYQb4bQ3KZ7bbZAyOTc1MDM3OTc1NjMyODA0ECcAAD3vFoc= </td>
	</tr>
	<tr class="row284">
		<td class="col0"> 18900 </td><td class="col1"> Android Backup <sup>*</sup> </td><td class="col2"> $ab$5*0*10000*b8900e4885ff9cad8f01ee1957a43bd633fea12491440514ae27aa83f2f5c006ec7e7fa0bce040add619919b4eb60608304b7d571a2ed87fd58c9ad6bc5fcf4c*7d254d93e16be9312fb1ccbfc6265c40cb0c5eab7b605a95a116e2383fb1cf12b688223f96221dcd2bf5410d4ca6f90e0789ee00157fa91658b42665d6b6844c*fc9f6be604d1c59ac32664ec2c5b9b30*00c4972149af3adcc235899e9d20611ea6e8de2212afcb9fcfefde7e35b691c2d0994eb47e4f9a260526ba47f4caea71af9c7fadcd5685d50126276f6acdd59966528b13ccc26036a0eaba2f2451aa64b05766d0edd03c988dcf87e2a9eec52d </td>
	</tr>
	<tr class="row285">
		<td class="col0"> 19000 </td><td class="col1"> QNX /etc/shadow (MD5) <sup>*</sup> </td><td class="col2"> @m@75f6f129f9c9e77b6b1b78f791ed764a@8741857532330050 </td>
	</tr>
	<tr class="row286">
		<td class="col0"> 19100 </td><td class="col1"> QNX /etc/shadow (SHA256) <sup>*</sup> </td><td class="col2"> @s@0b365cab7e17ee1e7e1a90078501cc1aa85888d6da34e2f5b04f5c614b882a93@5498317092471604 </td>
	</tr>
	<tr class="row287">
		<td class="col0"> 19200 </td><td class="col1"> QNX /etc/shadow (SHA512) <sup>*</sup> </td><td class="col2"> @S@715df9e94c097805dd1e13c6a40f331d02ce589765a2100ec7435e76b978d5efc364ce10870780622cee003c9951bd92ec1020c924b124cfff7e0fa1f73e3672@2257314490293159 </td>
	</tr>
	<tr class="row288">
		<td class="col0"> 19300 </td><td class="col1"> sha1($salt1.$pass.$salt2) <sup>*</sup> </td><td class="col2"> 630d2e918ab98e5fad9c61c0e4697654c4c16d73:18463812876898603420835420139870031762867:4449516425193605979760642927684590668549584534278112685644182848763890902699756869283142014018311837025441092624864168514500447147373198033271040848851687108629922695275682773136540885737874252666804716579965812709728589952868736177317883550827482248620334 </td>
	</tr>
	<tr class="row289">
		<td class="col0"> 19500 </td><td class="col1"> Ruby on Rails Restful-Authentication <sup>*</sup> </td><td class="col2"> d7d5ea3e09391da412b653ae6c8d7431ec273ea2:238769868762:8962783556527653675 </td>
	</tr>
	<tr class="row290">
		<td class="col0"> 19600 </td><td class="col1"> Kerberos 5 TGS-REP etype 17 (AES128-CTS-HMAC-SHA1-96) <sup>*</sup> </td><td class="col2"> $krb5tgs$17$user$realm$ae8434177efd09be5bc2eff8$90b4ce5b266821adc26c64f71958a475cf9348fce65096190be04f8430c4e0d554c86dd7ad29c275f9e8f15d2dab4565a3d6e21e449dc2f88e52ea0402c7170ba74f4af037c5d7f8db6d53018a564ab590fc23aa1134788bcc4a55f69ec13c0a083291a96b41bffb978f5a160b7edc828382d11aacd89b5a1bfa710b0e591b190bff9062eace4d26187777db358e70efd26df9c9312dbeef20b1ee0d823d4e71b8f1d00d91ea017459c27c32dc20e451ea6278be63cdd512ce656357c942b95438228e </td>
	</tr>
	<tr class="row291">
		<td class="col0"> 19700 </td><td class="col1"> Kerberos 5 TGS-REP etype 18 (AES256-CTS-HMAC-SHA1-96) <sup>*</sup> </td><td class="col2"> $krb5tgs$18$user$realm$8efd91bb01cc69dd07e46009$7352410d6aafd72c64972a66058b02aa1c28ac580ba41137d5a170467f06f17faf5dfb3f95ecf4fad74821fdc7e63a3195573f45f962f86942cb24255e544ad8d05178d560f683a3f59ce94e82c8e724a3af0160be549b472dd83e6b80733ad349973885e9082617294c6cbbea92349671883eaf068d7f5dcfc0405d97fda27435082b82b24f3be27f06c19354bf32066933312c770424eb6143674756243c1bde78ee3294792dcc49008a1b54f32ec5d5695f899946d42a67ce2fb1c227cb1d2004c0 </td>
	</tr>
	<tr class="row292">
		<td class="col0"> 19800 </td><td class="col1"> Kerberos 5, etype 17, Pre-Auth <sup>*</sup> </td><td class="col2"> $krb5pa$17$hashcat$HASHCATDOMAIN.COM$a17776abe5383236c58582f515843e029ecbff43706d177651b7b6cdb2713b17597ddb35b1c9c470c281589fd1d51cca125414d19e40e333 </td>
	</tr>
	<tr class="row293">
		<td class="col0"> 19900 </td><td class="col1"> Kerberos 5, etype 18, Pre-Auth <sup>*</sup> </td><td class="col2"> $krb5pa$18$hashcat$HASHCATDOMAIN.COM$96c289009b05181bfd32062962740b1b1ce5f74eb12e0266cde74e81094661addab08c0c1a178882c91a0ed89ae4e0e68d2820b9cce69770 </td>
	</tr>
	<tr class="row294">
		<td class="col0"> 20011 </td><td class="col1"> DiskCryptor SHA512 + XTS 512 bit (AES) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_aes.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_aes.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_aes.dc</a> </td>
	</tr>
	<tr class="row295">
		<td class="col0"> 20011 </td><td class="col1"> DiskCryptor SHA512 + XTS 512 bit (Twofish) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_twofish.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_twofish.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_twofish.dc</a> </td>
	</tr>
	<tr class="row296">
		<td class="col0"> 20011 </td><td class="col1"> DiskCryptor SHA512 + XTS 512 bit (Serpent) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_serpent.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_serpent.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_serpent.dc</a> </td>
	</tr>
	<tr class="row297">
		<td class="col0"> 20012 </td><td class="col1"> DiskCryptor SHA512 + XTS 1024 bit (AES-Twofish) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish.dc</a> </td>
	</tr>
	<tr class="row298">
		<td class="col0"> 20012 </td><td class="col1"> DiskCryptor SHA512 + XTS 1024 bit (Twofish-Serpent) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_twofish_serpent.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_twofish_serpent.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_twofish_serpent.dc</a> </td>
	</tr>
	<tr class="row299">
		<td class="col0"> 20012 </td><td class="col1"> DiskCryptor SHA512 + XTS 1024 bit (Serpent-AES) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_serpent_aes.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_serpent_aes.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_serpent_aes.dc</a> </td>
	</tr>
	<tr class="row300">
		<td class="col0"> 20013 </td><td class="col1"> DiskCryptor SHA512 + XTS 1536 bit (AES-Twofish-Serpent) <sup>*</sup> </td><td class="col2"> <a href="https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish_serpent.dc" class="urlextern" title="https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish_serpent.dc" rel="nofollow">https://hashcat.net/misc/example_hashes/dc/hashcat_aes_twofish_serpent.dc</a> </td>
	</tr>
	<tr class="row301">
		<td class="col0"> 20200 </td><td class="col1"> Python passlib pbkdf2-sha512 <sup>*</sup> </td><td class="col2"> $pbkdf2-sha512$25000$LyWE0HrP2RsjZCxlDGFMKQ$1vC5Ohk2mCS9b6akqsEfgeb4l74SF8XjH.SljXf3dMLHdlY1GK9ojcCKts6/asR4aPqBmk74nCDddU3tvSCJvw </td>
	</tr>
	<tr class="row302">
		<td class="col0"> 20300 </td><td class="col1"> Python passlib pbkdf2-sha256 <sup>*</sup> </td><td class="col2"> $pbkdf2-sha256$29000$x9h7j/Ge8x6DMEao1VqrdQ$kra3R1wEnY8mPdDWOpTqOTINaAmZvRMcYd8u5OBQP9A </td>
	</tr>
	<tr class="row303">
		<td class="col0"> 20400 </td><td class="col1"> Python passlib pbkdf2-sha1 <sup>*</sup> </td><td class="col2"> $pbkdf2$131000$r5WythYixPgfQ2jt3buXcg$8Kdr.QQEOaZIXNOrrru36I/.6Po </td>
	</tr>
	<tr class="row304">
		<td class="col0"> 20500 </td><td class="col1"> PKZIP Master Key <sup>*</sup> </td><td class="col2"> f1eff5c0368d10311dcfc419 </td>
	</tr>
	<tr class="row305">
		<td class="col0"> 20510 </td><td class="col1"> PKZIP Master Key (6 byte optimization) <sup>17</sup> <sup>*</sup> </td><td class="col2"> f1eff5c0368d10311dcfc419 </td>
	</tr>
	<tr class="row306">
		<td class="col0"> 20600 </td><td class="col1"> Oracle Transportation Management (SHA256) <sup>*</sup> </td><td class="col2"> otm_sha256:1000:1234567890:S5Q9Kc0ETY6ZPyQU+JYY60oFjaJuZZaSinggmzU8PC4= </td>
	</tr>
	<tr class="row307">
		<td class="col0"> 20710 </td><td class="col1"> sha256(sha256($pass).$salt) <sup>*</sup> </td><td class="col2"> bfede293ecf6539211a7305ea218b9f3f608953130405cda9eaba6fb6250f824:7218532375810603 </td>
	</tr>
	<tr class="row308">
		<td class="col0"> 20711 </td><td class="col1"> AuthMe sha256 </td><td class="col2"> $SHA$7218532375810603$bfede293ecf6539211a7305ea218b9f3f608953130405cda9eaba6fb6250f824 </td>
	</tr>
	<tr class="row309">
		<td class="col0"> 20800 </td><td class="col1"> sha256(md5($pass)) <sup>*</sup> </td><td class="col2"> 74ee1fae245edd6f27bf36efc3604942479fceefbadab5dc5c0b538c196eb0f1 </td>
	</tr>
	<tr class="row310">
		<td class="col0"> 20900 </td><td class="col1"> md5(sha1($pass).md5($pass).sha1($pass)) <sup>*</sup> </td><td class="col2"> 100b3a4fc1dc8d60d9bf40688d8b740a </td>
	</tr>
	<tr class="row311">
		<td class="col0"> 21000 </td><td class="col1"> BitShares v0.x - sha512(sha512_bin(pass)) <sup>*</sup> </td><td class="col2"> caec04bdf7c17f763a9ec7439f7c9abda112f1bfc9b1bb684fef9b6142636979b9896cfc236896d821a69a961a143dd19c96d59777258201f1bbe5ecc2a2ecf5 </td>
	</tr>
	<tr class="row312">
		<td class="col0"> 21100 </td><td class="col1"> sha1(md5($pass.$salt)) <sup>*</sup> </td><td class="col2"> aade80a61c6e3cd3cac614f47c1991e0a87dd028:6 </td>
	</tr>
	<tr class="row313">
		<td class="col0"> 21200 </td><td class="col1"> md5(sha1($salt).md5($pass)) <sup>*</sup> </td><td class="col2"> e69b7a7fe1bf2ad9ef116f79551ee919:baa038987e582431a6d </td>
	</tr>
	<tr class="row314">
		<td class="col0"> 21300 </td><td class="col1"> md5($salt.sha1($salt.$pass)) <sup>*</sup> </td><td class="col2"> 799dc7d9aa4d3f404cc21a4936dbdcde:68617368636174 </td>
	</tr>
	<tr class="row315">
		<td class="col0"> 21400 </td><td class="col1"> sha256(sha256_bin(pass)) <sup>*</sup> </td><td class="col2"> 0cc1b58a543f372327aa0281e97ab56e345267ee46feabf7709515debb7ec43c </td>
	</tr>
	<tr class="row316">
		<td class="col0"> 21500 </td><td class="col1"> SolarWinds Orion <sup>*</sup> </td><td class="col2"> $solarwinds$0$admin$fj4EBQewCQUZ7IYHl0qL8uj9kQSBb3m7N4u0crkKK0Uj9rbbAnSrBZMXO7oWx9KqL3sCzwncvPZ9hyDV9QCFTg== </td>
	</tr>
	<tr class="row317">
		<td class="col0"> 21600 </td><td class="col1"> Web2py pbkdf2-sha512 <sup>*</sup> </td><td class="col2"> pbkdf2(1000,20,sha512)$744943$c5f8cdef76e3327c908d8d96d4abdb3d8caba14c </td>
	</tr>
	<tr class="row318">
		<td class="col0"> 21700 </td><td class="col1"> Electrum Wallet (Salt-Type 4) <sup>*</sup> </td><td class="col2"> $electrum$4*03eae309d8bda5dcbddaae8145469193152763894b7260a6c4ba181b3ac2ed5653*8c594086a64dc87a9c1f8a69f646e31e8d3182c3c722def4427aa20684776ac26092c6f60bf2762e27adfa93fe1e952dcb8d6362224b9a371953aa3a2edb596ce5eb4c0879c4353f2cc515ec6c9e7a6defa26c5df346d18a62e9d40fcc606bc8c34322bf2212f77770a683788db0baf4cb43595c2a27fe5ff8bdcb1fd915bcd725149d8ee8f14c71635fecb04da5dde97584f4581ceb7d907dceed80ae5daa8352dda20b25fd6001e99a96b7cf839a36cd3f5656304e6998c18e03dd2fb720cb41386c52910c9cb83272c3d50f3a6ff362ab8389b0c21c75133c971df0a75b331796371b060b32fe1673f4a041d7ae08bbdeffb45d706eaf65f99573c07972701c97766b4d7a8a03bba0f885eb3845dfd9152286e1de1f93e25ce04c54712509166dda80a84c2d34652f68e6c01e662f8b1cc7c15103a4502c29332a4fdbdda470c875809e15aab3f2fcb061ee96992ad7e8ab9da88203e35f47d6e88b07a13b0e70ef76de3be20dc06facbddc1e47206b16b44573f57396265116b4d243e77d1c98bc2b28aa3ec0f8d959764a54ecdd03d8360ff2823577fe2183e618aac15b30c1d20986841e3d83c0bfabcedb7c27ddc436eb7113db927e0beae7522b04566631a090b214660152a4f4a90e19356e66ee7309a0671b2e7bfde82667538d193fc7e397442052c6c611b6bf0a04f629a1dc7fa9eb44bfad1bfc6a0bce9f0564c3b483737e447720b7fd038c9a961a25e9594b76bf8c8071c83fcacd689c7469f698ee4aee4d4f626a73e21ce4967e705e4d83e1145b4260330367d8341c84723a1b02567ffbab26aac3afd1079887b4391f05d09780fc65f8b4f68cd51391c06593919d7eafd0775f83045b8f5c2e59cef902ff500654ea29b7623c7594ab2cc0e05ffe3f10abc46c9c5dac824673c307dcbff5bc5f3774141ff99f6a34ec4dd8a58d154a1c72636a2422b8fafdef399dec350d2b91947448582d52291f2261d264d29399ae3c92dc61769a49224af9e7c98d74190f93eb49a44db7587c1a2afb5e1a4bec5cdeb8ad2aac9728d5ae95600c52e9f063c11cdb32b7c1d8435ce76fcf1fa562bd38f14bf6c303c70fb373d951b8a691ab793f12c0f3336d6191378bccaed32923bba81868148f029e3d5712a2fb9f610997549710716db37f7400690c8dfbed12ff0a683d8e4d0079b380e2fd856eeafb8c6eedfac8fb54dacd6bd8a96e9f8d23ea87252c1a7c2b53efc6e6aa1f0cc30fbaaf68ee7d46666afc15856669cd9baebf9397ff9f322cce5285e68a985f3b6aadce5e8f14e9f9dd16764bc4e9f62168aa265d8634ab706ed40b0809023f141c36717bd6ccef9ec6aa6bfd2d00bda9375c2fee9ebba49590a166*1b0997cf64bb2c2ff88cb87bcacd9729d404bd46db18117c20d94e67c946fedc </td>
	</tr>
	<tr class="row319">
		<td class="col0"> 21800 </td><td class="col1"> Electrum Wallet (Salt-Type 5) <sup>*</sup> </td><td class="col2"> $electrum$5*02170fee7c35f1ef3b229edc90fbd0793b688a0d6f41137a97aab2343d315cce16*94cf72d8f5d774932b414a3344984859e43721268d2eb35fa531de5a2fc7024b463c730a54f4f46229dd9fede5034b19ac415c2916e9c16b02094f845795df0c397ff76d597886b1f9e014ad1a8f64a3f617d9900aa645b3ba86f16ce542251fc22c41d93fa6bc118be96d9582917e19d2a299743331804cfc7ce2c035367b4cbcfb70adfb1e10a0f2795769f2165d8fd13daa8b45eeac495b5b63e91a87f63b42e483f84a881e49adecacf6519cb564694b42dd9fe80fcbc6cdb63cf5ae33f35255266f5c2524dd93d3cc15eba0f2ccdc3c109cc2d7e8f711b8b440f168caf8b005e8bcdfe694148e94a04d2a738f09349a96600bd8e8edae793b26ebae231022f24e96cb158db141ac40400a9e9ef099e673cfe017281537c57f82fb45c62bdb64462235a6eefb594961d5eb2c46537958e4d04250804c6e9f343ab7a0db07af6b8a9d1a6c5cfcd311b8fb8383ac9ed9d98d427d526c2f517fc97473bd87cb59899bd0e8fb8c57fa0f7e0d53daa57c972cf92764af4b1725a5fb8f504b663ec519731929b3caaa793d8ee74293eee27d0e208a60e26290bc546e6fa9ed865076e13febfea249729218c1b5752e912055fbf993fbac5df2cca2b37c5e0f9c30789858ceeb3c482a8db123966775aeed2eee2fc34efb160d164929f51589bff748ca773f38978bff3508d5a7591fb2d2795df983504a788071f469d78c88fd7899cabbc5804f458653d0206b82771a59522e1fa794d7de1536c51a437f5d6df5efd6654678e5794ca429b5752e1103340ed80786f1e9da7f5b39af628b2212e4d88cd36b8a7136d50a6b6e275ab406ba7c57cc70d77d01c4c16e9363901164fa92dc9e9b99219d5376f24862e775968605001e71b000e2c7123b4b43f3ca40db17efd729388782e46e64d43ccb947db4eb1473ff1a3836b74fe312cd1a33b73b8b8d80c087088932277773c329f2f66a01d6b3fc1e651c56959ebbed7b14a21b977f3acdedf1a0d98d519a74b50c39b3052d840106da4145345d86ec0461cddafacc2a4f0dd646457ad05bf04dcbcc80516a5c5ed14d2d639a70e77b686f19cbfb63f546d81ae19cc8ba35cce3f3b5b9602df25b678e14411fecec87b8347f5047513df415c6b1a3d39871a6bcb0f67d9cf8311596deae45fd1d84a04fd58f1fd55c5156b7309af09094c99a53674809cb87a45f95a2d69f9997a38085519cb4e056f9efd56672a2c1fe927d5ea8eec25b8aff6e56f9a2310f1a481daf407b8adf16201da267c59973920fd21bb087b88123ef98709839d6a3ee34efb8ccd5c15ed0e46cff3172682769531164b66c8689c35a26299dd26d09233d1f64f9667474141cf9c6a6de7f2bc52c3bb44cfe679ff4b912c06df406283836b3581773cb76d375304f46239da5996594a8d03b14c02f1b35a432dc44a96331242ae31174*33a7ee59d6d17ed1ee99dc0a71771227e6f3734b17ba36eb589bdced56244135 </td>
	</tr>
	<tr class="row320">
		<td class="col0"> 22000 </td><td class="col1"> WPA-PBKDF2-PMKID+EAPOL <sup>1</sup><sup>*</sup> </td><td class="col2"> WPA*01*4d4fe7aac3a2cecab195321ceb99a7d0*fc690c158264*f4747f87f9f4*686173686361742d6573736964*** </td>
	</tr>
	<tr class="row321">
		<td class="col0"> 22001 </td><td class="col1"> WPA-PMK-PMKID+EAPOL <sup>18</sup><sup>*</sup> </td><td class="col2"> WPA*01*5ce7ebe97a1bbfeb2822ae627b726d5b*27462da350ac*accd10fb464e*686173686361742d6573736964*** </td>
	</tr>
	<tr class="row322">
		<td class="col0"> 22100 </td><td class="col1"> BitLocker <sup>*</sup> </td><td class="col2"> $bitlocker$1$16$6f972989ddc209f1eccf07313a7266a2$1048576$12$3a33a8eaff5e6f81d907b591$60$316b0f6d4cb445fb056f0e3e0633c413526ff4481bbf588917b70a4e8f8075f5ceb45958a800b42cb7ff9b7f5e17c6145bf8561ea86f52d3592059fb </td>
	</tr>
	<tr class="row323">
		<td class="col0"> 22200 </td><td class="col1"> Citrix NetScaler (SHA512) <sup>*</sup> </td><td class="col2"> 2f9282ade42ce148175dc3b4d8b5916dae5211eee49886c3f7cc768f6b9f2eb982a5ac2f2672a0223999bfd15349093278adf12f6276e8b61dacf5572b3f93d0b4fa886ce </td>
	</tr>
	<tr class="row324">
		<td class="col0"> 22300 </td><td class="col1"> sha256($salt.$pass.$salt) <sup>*</sup> </td><td class="col2"> 755a8ce4e0cf0baee41d714aa35c9fca803106608f718f973eab006578285007:11265 </td>
	</tr>
	<tr class="row325">
		<td class="col0"> 22400 </td><td class="col1"> AES Crypt (SHA256) <sup>*</sup> </td><td class="col2"> $aescrypt$1*efc648908ca7ec727f37f3316dfd885c*eff5c87a35545406a57b56de57bd0554*3a66401271aec08cbd10cf2070332214093a33f36bd0dced4a4bb09fab817184*6a3c49fea0cafb19190dc4bdadb787e73b1df244c51780beef912598bd3bdf7e </td>
	</tr>
	<tr class="row326">
		<td class="col0"> 22500 </td><td class="col1"> MultiBit Classic .key (MD5) <sup>*</sup> </td><td class="col2"> $multibit$1*e5912fe5c84af3d5*5f0391c219e8ef62c06505b1f6232858f5bcaa739c2b471d45dd0bd8345334de </td>
	</tr>
	<tr class="row327">
		<td class="col0"> 22600 </td><td class="col1"> Telegram Desktop App Passcode (PBKDF2-HMAC-SHA1) <sup>*</sup> </td><td class="col2"> $telegram$1*4000*913a7e42143b4eed0fb532dacfa04e3a0eae036ae66dd02de76323046c575531*cde5f7a3bda3812b4a3cd4df1269c6be18ca7536981522c251cab531c274776804634cdca5313dc8beb9895f903a40d874cd50dbb82e5e4d8f264820f3f2e2111a5831e1a2f16b1a75b2264c4b4485dfe0f789071130160af205f9f96aef378ee05602de2562f8c3b136a75ea01f54f4598af93f9e7f98eb66a5fd3dabaa864708fe0e84b59b77686974060f1533e3acc5367bc493915b5614603cf5601cfa0a6b8eae4c4bd24948176dd7ff470bc0863f35fdfce31a667c70e37743f662bc9c5ec86baff3ebb6bf7de96bcdfaca18baf9617a979424f792ef6e65e346ea2cbc1d53377f47c3fc681d7eda8169e6e20cd6a22dd94bf24933b8ffc4878216fa9edc7c72a073446a14b63e12b223f840217a7eac51b6afcc15bfa12afd3e85d3bd </td>
	</tr>
	<tr class="row328">
		<td class="col0"> 99999 </td><td class="col1"> Plaintext </td><td class="col2"> hashcat </td>
	</tr>
</tbody></table></div>

<p>
<sup>*</sup> In beta or not yet released<br>

<sup>1</sup> Password: “hashcat!”<br>

<sup>2</sup> Rounds=[# of iterations] is <strong>optional</strong> here, after signature, e.g. $5$rounds=5000 <br>

<sup>3</sup> As in <sup>2</sup> but the number of rounds <strong>must</strong> be specified<br>

<sup>4</sup> The hash used here is <strong>not</strong> the one sent via e.g. the web interface to LastPass servers (pbkdf2_sha256_hex (pbkdf2_sha256 ($pass, $email, $iterations), $pass, 1) but instead the one stored (by e.g. your browser or the pocket version) to disk. For instance, Opera and Chrome store the hash in local SQLite databases; Firefox uses files ending with “lpall.slps” - for Linux: 2nd line is interesting / base64 decode it; for Windows, see <a href="https://hashcat.net/forum/thread-2701-post-16111.html#pid16111" class="urlextern" title="https://hashcat.net/forum/thread-2701-post-16111.html#pid16111" rel="nofollow">here</a> - and_key.itr<br>

<sup>5</sup> You can consider the second part as a “salt”. If it is equal to 00000000, the CRC32 code will be considered as “not salted”<br>

<sup>6</sup> The raw sha256 output is used for base64() encoding (not the hexadecimal output)<br>

<sup>7</sup> The format is hash:salt:id<br>

<sup>8</sup> Password: “hashcat1”<br>

<sup>9</sup> Password: “hashcat1hashcat1hashcat1”<br>

<sup>10</sup> This file actually contains several examples of the different hash+cipher combinations. The password is stored in the pw file.<br>

<sup>11</sup> You can use <a href="https://github.com/philsmd/itunes_backup2hashcat/" class="urlextern" title="https://github.com/philsmd/itunes_backup2hashcat/" rel="nofollow">itunes_backup2hashcat</a> to extract the hashes from the Manifest.plist file<br>

<sup>12</sup> Password: “hashcat!!!”. Min/max password length is exactly 10 characters/bytes.<br>

<sup>13</sup> You can use <a href="https://github.com/Fist0urs/AxSuite" class="urlextern" title="https://github.com/Fist0urs/AxSuite" rel="nofollow">AxSuite by Fist0urs</a> to retrieve the hashes.<br>

<sup>14</sup> Password: a288fcf0caaacda9a9f58633ff35e8992a01d9c10ba5e02efdf8cb5d730ce7bc<br>

<sup>15</sup> Password: 5b13d4babb3714ccc62c9f71864bc984efd6a55f237c7a87fc2151e1ca658a9d<br>

<sup>16</sup> PIM: 500<br>

<sup>17</sup> full password in output is hashcat, but input provided must be without the first 6 bytes (therefore just: t)<br>

<sup>18</sup> 88f43854ae7b1624fc2ab7724859e795130f4843c7535729e819cf92f39535dc<br>

<sup>19</sup> use this SQL query to extract the hashes:<br>

</p>
<pre class="code">SELECT user, CONCAT('$mysql',LEFT(authentication_string,6),'*',INSERT(HEX(SUBSTR(authentication_string,8)),41,0,'*')) AS hash FROM user WHERE plugin = 'caching_sha2_password' AND authentication_string NOT LIKE '%INVALIDSALTANDPASSWORD%';</pre>

<p>
<br>

</p>

</div>

<h1 class="sectionedit4" id="specific_hash_types">Specific hash types</h1>
<div class="level1">

<p>
These hash types are usually only found on a specific platform.
</p>
<div class="plugin_tablelayout_placeholder" data-tablelayout="{&quot;colwidth&quot;:[&quot;60px&quot;,&quot;340px&quot;,&quot;540px&quot;],&quot;rowsHeaderSource&quot;:&quot;1&quot;,&quot;rowsVisible&quot;:&quot;0&quot;,&quot;float&quot;:&quot;left&quot;}"></div><div class="table sectionedit5"><table class="inline">
	<thead>
	<tr class="row0">
		<th class="col0"> Hash-Mode </th><th class="col1"> Hash-Name </th><th class="col2"> Example </th>
	</tr>
	</thead>
	<tbody><tr class="row1">
		<td class="col0"> 11 </td><td class="col1"> Joomla &lt; 2.5.18 </td><td class="col2"> 19e0e8d91c722e7091ca7a6a6fb0f4fa:54718031842521651757785603028777 </td>
	</tr>
	<tr class="row2">
		<td class="col0"> 12 </td><td class="col1"> PostgreSQL </td><td class="col2"> a6343a68d964ca596d9752250d54bb8a:postgres </td>
	</tr>
	<tr class="row3">
		<td class="col0"> 21 </td><td class="col1"> osCommerce, xt:Commerce </td><td class="col2"> 374996a5e8a5e57fd97d893f7df79824:36 </td>
	</tr>
	<tr class="row4">
		<td class="col0"> 22 </td><td class="col1"> Juniper NetScreen/SSG (ScreenOS) </td><td class="col2"> nNxKL2rOEkbBc9BFLsVGG6OtOUO/8n:user </td>
	</tr>
	<tr class="row5">
		<td class="col0"> 23 </td><td class="col1"> Skype </td><td class="col2"> 3af0389f093b181ae26452015f4ae728:user </td>
	</tr>
	<tr class="row6">
		<td class="col0"> 101 </td><td class="col1"> nsldap, SHA-1(Base64), Netscape LDAP SHA </td><td class="col2"> {SHA}uJ6qx+YUFzQbcQtyd2gpTQ5qJ3s= </td>
	</tr>
	<tr class="row7">
		<td class="col0"> 111 </td><td class="col1"> nsldaps, SSHA-1(Base64), Netscape LDAP SSHA </td><td class="col2"> {SSHA}AZKja92fbuuB9SpRlHqaoXxbTc43Mzc2MDM1Ng== </td>
	</tr>
	<tr class="row8">
		<td class="col0"> 112 </td><td class="col1"> Oracle S: Type (Oracle 11+) </td><td class="col2"> ac5f1e62d21fd0529428b84d42e8955b04966703:38445748184477378130 </td>
	</tr>
	<tr class="row9">
		<td class="col0"> 121 </td><td class="col1"> SMF (Simple Machines Forum) &gt; v1.1 </td><td class="col2"> ecf076ce9d6ed3624a9332112b1cd67b236fdd11:17782686 </td>
	</tr>
	<tr class="row10">
		<td class="col0"> 122 </td><td class="col1"> OSX v10.4, OSX v10.5, OSX v10.6 </td><td class="col2"> 1430823483d07626ef8be3fda2ff056d0dfd818dbfe47683 </td>
	</tr>
	<tr class="row11">
		<td class="col0"> 124 </td><td class="col1"> Django (SHA-1) </td><td class="col2"> sha1$fe76b$02d5916550edf7fc8c886f044887f4b1abf9b013 </td>
	</tr>
	<tr class="row12">
		<td class="col0"> 125 </td><td class="col1"> ArubaOS </td><td class="col2"> 5387280701327dc2162bdeb451d5a465af6d13eff9276efeba </td>
	</tr>
	<tr class="row13">
		<td class="col0"> 131 </td><td class="col1"> MSSQL (2000) </td><td class="col2"> 0x01002702560500000000000000000000000000000000000000008db43dd9b1972a636ad0c7d4b8c515cb8ce46578 </td>
	</tr>
	<tr class="row14">
		<td class="col0"> 132 </td><td class="col1"> MSSQL (2005) </td><td class="col2"> 0x010018102152f8f28c8499d8ef263c53f8be369d799f931b2fbe </td>
	</tr>
	<tr class="row15">
		<td class="col0"> 133 </td><td class="col1"> PeopleSoft </td><td class="col2"> uXmFVrdBvv293L9kDR3VnRmx4ZM= </td>
	</tr>
	<tr class="row16">
		<td class="col0"> 141 </td><td class="col1"> Episerver 6.x &lt; .NET 4 </td><td class="col2"> $episerver$*0*bEtiVGhPNlZpcUN4a3ExTg==*utkfN0EOgljbv5FoZ6+AcZD5iLk </td>
	</tr>
	<tr class="row17">
		<td class="col0"> 1411 </td><td class="col1"> SSHA-256(Base64), LDAP {SSHA256} </td><td class="col2"> {SSHA256}OZiz0cnQ5hgyel3Emh7NCbhBRCQ+HVBwYplQunHYnER7TLuV </td>
	</tr>
	<tr class="row18">
		<td class="col0"> 1421 </td><td class="col1"> hMailServer </td><td class="col2"> 8fe7ca27a17adc337cd892b1d959b4e487b8f0ef09e32214f44fb1b07e461c532e9ec3 </td>
	</tr>
	<tr class="row19">
		<td class="col0"> 1441 </td><td class="col1"> Episerver 6.x &gt;= .NET 4 </td><td class="col2"> $episerver$*1*MDEyMzQ1Njc4OWFiY2RlZg==*lRjiU46qHA7S6ZE7RfKUcYhB85ofArj1j7TrCtu3u6Y </td>
	</tr>
	<tr class="row20">
		<td class="col0"> 1711 </td><td class="col1"> SSHA-512(Base64), LDAP {SSHA512} </td><td class="col2"> {SSHA512}ALtwKGBdRgD+U0fPAy31C28RyKYx7+a8kmfksccsOeLknLHv2DBXYI7TDnTolQMBuPkWDISgZr2cHfnNPFjGZTEyNDU4OTkw </td>
	</tr>
	<tr class="row21">
		<td class="col0"> 1722 </td><td class="col1"> OSX v10.7 </td><td class="col2"> 648742485c9b0acd786a233b2330197223118111b481abfa0ab8b3e8ede5f014fc7c523991c007db6882680b09962d16fd9c45568260531bdb34804a5e31c22b4cfeb32d </td>
	</tr>
	<tr class="row22">
		<td class="col0"> 1731 </td><td class="col1"> MSSQL (2012, 2014) </td><td class="col2"> 0x02000102030434ea1b17802fd95ea6316bd61d2c94622ca3812793e8fb1672487b5c904a45a31b2ab4a78890d563d2fcf5663e46fe797d71550494be50cf4915d3f4d55ec375 </td>
	</tr>
	<tr class="row23">
		<td class="col0"> 2611 </td><td class="col1"> vBulletin &lt; v3.8.5 </td><td class="col2"> 16780ba78d2d5f02f3202901c1b6d975:568 </td>
	</tr>
	<tr class="row24">
		<td class="col0"> 2612 </td><td class="col1"> PHPS </td><td class="col2"> $PHPS$34323438373734$5b07e065b9d78d69603e71201c6cf29f </td>
	</tr>
	<tr class="row25">
		<td class="col0"> 2711 </td><td class="col1"> vBulletin &gt;= v3.8.5 </td><td class="col2"> bf366348c53ddcfbd16e63edfdd1eee6:181264250056774603641874043270 </td>
	</tr>
	<tr class="row26">
		<td class="col0"> 2811 </td><td class="col1"> IPB2+ (Invision Power Board), MyBB 1.2+ </td><td class="col2"> 8d2129083ef35f4b365d5d87487e1207:47204 </td>
	</tr>
	<tr class="row27">
		<td class="col0"> 3711 </td><td class="col1"> MediaWiki B type </td><td class="col2"> $B$56668501$0ce106caa70af57fd525aeaf80ef2898 </td>
	</tr>
	<tr class="row28">
		<td class="col0"> 4521 </td><td class="col1"> Redmine </td><td class="col2"> 1fb46a8f81d8838f46879aaa29168d08aa6bf22d:3290afd193d90e900e8021f81409d7a9 </td>
	</tr>
	<tr class="row29">
		<td class="col0"> 4522 </td><td class="col1"> PunBB </td><td class="col2"> 4a2b722cc65ecf0f7797cdaea4bce81f66716eef:653074362104 </td>
	</tr>
	<tr class="row30">
		<td class="col0"> 4711 </td><td class="col1"> Huawei sha1(md5($pass).$salt) </td><td class="col2"> 53c724b7f34f09787ed3f1b316215fc35c789504:hashcat1 </td>
	</tr>
	<tr class="row31">
		<td class="col0"> 7401 </td><td class="col1"> MySQL $A$ (sha256crypt) <sup>19</sup> <sup>*</sup> </td><td class="col2"> $mysql$A$005*F9CC98CE08892924F50A213B6BC571A2C11778C5*625479393559393965414D45316477456B484F41316E64484742577A2E3162785353526B7554584647562F </td>
	</tr>
	<tr class="row32">
		<td class="col0"> 12001 </td><td class="col1"> Atlassian (PBKDF2-HMAC-SHA1)</td><td class="col2"> {PKCS5S2}NzIyNzM0NzY3NTIwNjI3MdDDis7wPxSbSzfFqDGf7u/L00kSEnupbz36XCL0m7wa </td>
	</tr>
	<tr class="row33">
		<td class="col0"> 22301 </td><td class="col1"> Telegram Mobile App Passcode (SHA256) <sup>*</sup> </td><td class="col2"> $telegram$0*518c001aeb3b4ae96c6173be4cebe60a85f67b1e087b045935849e2f815b5e41*25184098058621950709328221838128 </td>
	</tr>
</tbody></table></div>

</div>

<h1 class="sectionedit6" id="legacy_hash_types">Legacy hash types</h1>
<div class="level1">

<p>
These hash types are only supported in <a href="/wiki/doku.php?id=hashcat-legacy" class="wikilink1" title="hashcat-legacy">hashcat-legacy</a> or <a href="/wiki/doku.php?id=oclhashcat" class="wikilink1" title="oclhashcat">oclHashcat</a>.
</p>
<div class="plugin_tablelayout_placeholder" data-tablelayout="{&quot;colwidth&quot;:[&quot;60px&quot;,&quot;340px&quot;,&quot;540px&quot;],&quot;rowsHeaderSource&quot;:&quot;1&quot;,&quot;rowsVisible&quot;:&quot;0&quot;,&quot;float&quot;:&quot;left&quot;}"></div><div class="table sectionedit7"><table class="inline">
	<thead>
	<tr class="row0">
		<th class="col0"> Hash-Mode </th><th class="col1"> Hash-Name </th><th class="col2"> Example </th>
	</tr>
	</thead>
	<tbody><tr class="row1">
		<td class="col0"> <del>123</del> </td><td class="col1"> <del>EPi</del> </td><td class="col2"> 0x326C6D7B4E4F794B79474E36704F35723958397163735263516265456E31 0xAFC55E260B8F45C0C6512BCE776C1AD8312B56E6 </td>
	</tr>
	<tr class="row2">
		<td class="col0"> <del>190</del> </td><td class="col1"> <del>sha1(LinkedIn)</del> <sup>2</sup> </td><td class="col2 leftalign"> b89eaac7e61417341b710b727768294d0e6a277b  </td>
	</tr>
	<tr class="row3">
		<td class="col0"> <del>1431</del> </td><td class="col1"> <del>base64(sha256(unicode($pass)))</del> <sup>1</sup> </td><td class="col2"> npKD5jP0p6QtOryTcBFVvor+VmDaJMh1jn01M+Ly3II= </td>
	</tr>
	<tr class="row4">
		<td class="col0"> <del>3300</del> </td><td class="col1"> <del>MD5(Sun)</del> <sup>1</sup> </td><td class="col2"> $md5$rounds=904$iPPKEBnEkp3JV8uX$0L6m7rOFTVFn.SGqo2M9W1 </td>
	</tr>
	<tr class="row5">
		<td class="col0"> <del>3500</del> </td><td class="col1"> <del>md5(md5(md5($pass)))</del> <sup>1</sup> </td><td class="col2"> 9882d0778518b095917eb589f6998441 </td>
	</tr>
	<tr class="row6">
		<td class="col0"> <del>3610</del> </td><td class="col1"> <del>md5(md5($salt).$pass)</del> <sup>1</sup> </td><td class="col2"> 7b57255a15958ef898543ea6cc3313bc:1234 </td>
	</tr>
	<tr class="row7">
		<td class="col0"> <del>3720</del> </td><td class="col1"> <del>md5($pass.md5($salt))</del> <sup>1</sup> </td><td class="col2"> 10ce488714fdbde9453670e0e4cbe99c:1234 </td>
	</tr>
	<tr class="row8">
		<td class="col0"> <del>3721</del> </td><td class="col1"> <del>WebEdition <abbr title="Content Management System">CMS</abbr></del> <sup>1</sup> </td><td class="col2"> fa01af9f0de5f377ae8befb03865178e:​5678 </td>
	</tr>
	<tr class="row9">
		<td class="col0"> <del>4210</del> </td><td class="col1"> <del>md5($username.0.$pass)</del> <sup>1</sup> </td><td class="col2"> 09ea048c345ad336ebe38ae5b6c4de24:1234 </td>
	</tr>
	<tr class="row10">
		<td class="col0"> <del>4600</del> </td><td class="col1"> <del>sha1(sha1(sha1($pass)))</del> <sup>1</sup> </td><td class="col2"> dc57f246485e62d99a5110afc9264b4ccbfcf3cc </td>
	</tr>
</tbody></table></div>

<p>
<sup>1</sup> Supported in <a href="/wiki/doku.php?id=hashcat-legacy" class="wikilink1" title="hashcat-legacy">hashcat-legacy</a><br>

<sup>2</sup> Supported in <a href="/wiki/doku.php?id=oclhashcat" class="wikilink1" title="oclhashcat">oclHashcat</a><br>

</p>

</div>

<h1 class="sectionedit8" id="superseded_hash_types">Superseded hash types</h1>
<div class="level1">

<p>
These hash types used to be in some version of hashcat, but were removed or replaced.
</p>
<div class="plugin_tablelayout_placeholder" data-tablelayout="{&quot;colwidth&quot;:[&quot;60px&quot;,&quot;340px&quot;,&quot;540px&quot;],&quot;rowsHeaderSource&quot;:&quot;1&quot;,&quot;rowsVisible&quot;:&quot;0&quot;,&quot;float&quot;:&quot;left&quot;}"></div><div class="table sectionedit9"><table class="inline">
	<thead>
	<tr class="row0">
		<th class="col0"> Hash-Mode </th><th class="col1"> Hash-Name </th><th class="col2"> Example </th><td class="col3"></td>
	</tr>
	</thead>
	<tbody><tr class="row1">
		<td class="col0"> 5000 </td><td class="col1"> SHA-3 (Keccak) </td><td class="col2"> 203f88777f18bb4ee1226627b547808f38d90d3e106262b5de9ca943b57137b6 </td><td class="col3"> replaced by specific Keccak types in hashcat 5.0.0</td>
	</tr>
</tbody></table></div>

</div>

    <!-- wikipage stop -->
  </div>
