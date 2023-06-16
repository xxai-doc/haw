<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Manaʻo ʻia e hoʻokomo i nā nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mua, a laila `direnv allow` ma hope o ke komo ʻana i ka papa kuhikuhi (e hoʻokō ʻia [ka .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) ma hope o ke komo ʻana i ka papa kuhikuhi).

ʻO ka manaʻo: unuhi Pākē i ka ʻōlelo Kepanī, Kōlea, Pelekania, unuhi Pelekane i nā ʻōlelo ʻē aʻe. Inā makemake ʻoe e kākoʻo i ka Pākē a me ka ʻōlelo Pelekania, hiki iā ʻoe ke kākau `zh: en` .

## code hope-mua

* [code hope-mua](https://github.com/xxai-art/web)
* [Nā pūʻolo ʻōlelo no ka pūnaewele holoʻokoʻa](https://github.com/xxai-art/web/tree/main/i18n)
* [Nā pūʻolo ʻōlelo no nā modula e komo](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Paenaewele Nā Palapala ʻōlelo he nui](https://github.com/xxai-doc)

ʻO ka ʻōlelo hoʻonohonoho mua ʻo [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , e hoʻohui i kekahi mau hiʻohiʻona e pili ana i ka syntax coffeescript, e ʻike iā [./coffee_plus.md](./coffee_plus.md) .

## Internationalization o nā pūnaewele a me nā palapala

E kūkulu ma luna o nā papahana 3 aʻe

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  ʻO ka suffix ʻo `.mdt` , hiki iā ʻoe ke hoʻohana i ka syntax e like me `<+ ./coffee_plus/import.js>` e kuhikuhi i nā faila waho, a hoʻohua i ka markdown me ka suffix `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  ʻAʻole unuhi ʻo Markdown i nā code a me nā loulou, a e hūnā i nā huaʻōlelo unuhi. Inā hoʻololi ʻia ka unuhi akā ʻaʻole i hoʻololi ʻia ka kikokikona kumu, ʻaʻole e hoʻololi hou ʻia ka unuhi ʻana.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Nā waihona ʻōlelo no ka unuhi ʻana i nā pūnaewele i haku ʻia `yaml` .

### Nā ʻōlelo aʻoaʻo no ka unuhi ʻana i ka palapala

E ʻike i ka waihona code [xxai-art/doc](https://github.com/xxai-art/doc)

Manaʻo ʻia e hoʻokomo i nā nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) mua, a laila `direnv allow` ma hope o ke komo ʻana i ka papa kuhikuhi (e hoʻokō ʻia [ka .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) ma hope o ke komo ʻana i ka papa kuhikuhi).

I mea e pale aku ai i ka waihona code nui i unuhi ʻia i loko o nā haneli mau ʻōlelo, ua hana wau i kahi waihona code kaʻawale no kēlā me kēia ʻōlelo a hana i kahi hui e mālama i ka waihona code.

Ke hoʻonohonoho ʻana i ka hoʻololi kaiapuni `GITHUB_ACCESS_TOKEN` a laila e holo ana i [ka create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) e hana ʻakomi i ka waihona code.

ʻOiaʻiʻo, hiki iā ʻoe ke hoʻokomo i loko o kahi kumu code.

Kuhikuhi palapala unuhi [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Ua unuhi ʻia ka code script penei:

ʻO [ka bunx](https://bun.sh/docs/cli/bunx) kahi pani no npx, ʻoi aku ka wikiwiki. ʻOiaʻiʻo, inā ʻaʻole ʻoe i hoʻokomo i ka bun, hiki iā ʻoe ke hoʻohana i `npx` ma kahi.

`bunx mdt zh` renders `.mdt` i loko o ka zh directory like `.md` , e ike i ka 2 loulou ma lalo nei.

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` ke code kumu no ka unuhi (inā he `nodejs` kāu i hoʻokomo ʻia, akā ʻaʻole hoʻokomo ʻia `bun` a me `direnv` , hiki iā ʻoe ke holo i `npx i18n` e unuhi).

E hoʻopau ia [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , ʻo ka hoʻonohonoho ʻana o `i18n.yml` i kēia palapala penei:

```
en:
zh: ja ko en
```

ʻO ka manaʻo: unuhi Pākē i ka ʻōlelo Kepanī, Kōlea, Pelekania, unuhi Pelekane i nā ʻōlelo ʻē aʻe. Inā makemake ʻoe e kākoʻo i ka Pākē a me ka ʻōlelo Pelekania, hiki iā ʻoe ke kākau `zh: en` .

ʻO ka hope ʻo [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , nāna e unuhi i ka ʻike ma waena o ke poʻo inoa nui a me ka poʻomanaʻo mua o `README.md` o kēlā me kēia ʻōlelo e hoʻopuka i kahi helu `README.md` . He maʻalahi loa ke code, hiki iā ʻoe ke nānā iā ʻoe iho.

Hoʻohana ʻia ʻo Google API no ka unuhi manuahi. Inā ʻaʻole hiki iā ʻoe ke komo iā Google, e ʻoluʻolu e hoʻonohonoho a hoʻonohonoho i kahi koho, e like me:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

E hoʻopuka ka unuhi unuhi i kahi huna huna i unuhi ʻia ma ka papa kuhikuhi `.i18n` , e ʻoluʻolu e nānā me `git status` a hoʻohui i ka waihona code no ka pale ʻana i ka unuhi hou ʻana.

E ʻoluʻolu e holo i `bunx i18n` i kēlā me kēia manawa āu e hoʻololi ai i ka unuhi e hoʻohou i ka huna huna.

Inā hoʻololi ʻia ka kikokikona kumu a me ka unuhi i ka manawa like, huikau ka huna huna, no laila inā makemake ʻoe e hoʻololi, hiki iā ʻoe ke hoʻololi i hoʻokahi wale nō, a laila holo i `bunx i18n` e hoʻonui i ka cache.
