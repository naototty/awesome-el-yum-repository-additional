# awesome-el-yum-repository-additional
awesome EL(centos,redhat) additional yum repository

[original](https://qiita.com/bezeklik/items/9766003c19f9664602fe)

yumリポジトリ一追加リスト 完全版
様々な yum のリポジトリーを収集した。他にあればコメントで教えてください。

## とりあえずコピペ用
#### 汎用

| リポジトリー | コマンド |
|-----------|--------|
| **[EPEL](https://fedoraproject.org/wiki/EPEL/ja)** | `yum install epel-release` |
| **[Remi](http://rpms.famillecollet.com/)** | `yum install http://rpms.famillecollet.com/enterprise/remi-release-7.rpm`<br>`yum install http://rpms.famillecollet.com/enterprise/remi-release-6.rpm` |
| **[RepoForge](http://repoforge.org/)**<br>(旧RPMForge) | [RPMForge (RepoForge) 終了のお知らせ](http://qiita.com/bezeklik/items/ba4ccd806ae39d35f782) |
| **Webtatic** | `yum install https://mirror.webtatic.com/yum/el7/webtatic-release.rpm`<br>`yum install https://mirror.webtatic.com/yum/el6/latest.rpm` |
| **IUS**  | `curl -s https://setup.ius.io/ `&#124;` sh` |
| **Atomic** | `curl -s http://www.atomicorp.com/installers/atomic `&#124;` sh` |
| **CentOS-SCL** | `yum install centos-release-scl` (CentOS 7)<br>`yum install centos-release-SCL` (CentOS 6) |
| **ELRepo** | `yum install http://www.elrepo.org/elrepo-release-7.0-2.el7.elrepo.noarch.rpm`<br>`yum install http://www.elrepo.org/elrepo-release-6-6.el6.elrepo.noarch.rpm` |
|**[Lux](http://repo.iotti.biz/)**|`yum install http://repo.iotti.biz/CentOS/7/noarch/lux-release-7-1.noarch.rpm`<br>`yum install http://repo.iotti.biz/CentOS/6/noarch/lux-release-6-3.noarch.rpm`(未検証)|
|**[PUIAS](https://springdale.math.ias.edu/wiki/YumRepositories6)**|`yum install http://puias.math.ias.edu/data/puias/6/x86_64/os/Packages/springdale-core-6-2.sdl6.10.noarch.rpm`(未検証)<br>`yum install http://puias.math.ias.edu/data/puias/6/x86_64/os/Packages/springdale-addons-6-2.sdl6.10.noarch.rpm`(未検証)|
|**[Psychotic Ninja](http://wiki.psychotic.ninja/index.php?title=Main_Page)**|`yum install http://packages.psychotic.ninja/7/base/x86_64/RPMS/psychotic-release-1.0.0-1.el7.psychotic.noarch.rpm`(未検証)|
|**[CERT Forensics Tools](https://forensics.cert.org/)**|`yum install https://forensics.cert.org/cert-forensics-tools-release-el7.rpm`(未検証)|
|**[End Point](https://packages.endpoint.com/)**|`yum install https://packages.endpoint.com/rhel/7/os/x86_64/endpoint-repo-1.7-1.x86_64.rpm`(未検証)|
|**[Ghettoforge](http://ghettoforge.org/index.php/Main_Page)**|`yum install http://mirror.symnds.com/distributions/gf/el/7/gf/x86_64/gf-release-7-10.gf.el7.noarch.rpm`(未検証)|

#### DB
| リポジトリー | コマンド |
|-----------|--------|
| **[MySQL](https://dev.mysql.com/downloads/repo/yum/)** | `yum install http://dev.mysql.com/get/mysql57-community-release-el7-9.noarch.rpm`<br>`http://dev.mysql.com/get/mysql-community-release-el7-5.noarch.rpm`<br>`yum install http://dev.mysql.com/get/mysql57-community-release-el6-9.noarch.rpm`<br>`http://dev.mysql.com/get/mysql-community-release-el6-5.noarch.rpm` |
| **MariaDB** | https://downloads.mariadb.org/mariadb/repositories/ |
| **[PostgreSQL](http://yum.postgresql.org/)** | `yum install https://download.postgresql.org/pub/repos/yum/9.6/redhat/rhel-7-x86_64/pgdg-centos96-9.6-3.noarch.rpm`<br>`yum install https://download.postgresql.org/pub/repos/yum/9.6/redhat/rhel-6-x86_64/pgdg-centos96-9.6-3.noarch.rpm` |
| **MongoDB** | https://docs.mongodb.org/manual/tutorial/install-mongodb-on-red-hat/#configure-the-package-management-system-yum |

#### その他
| リポジトリー | コマンド |
|-----------|--------|
| **nginx** | `yum install http://nginx.org/packages/centos/7/noarch/RPMS/nginx-release-centos-7-0.el7.ngx.noarch.rpm`<br>`yum install http://nginx.org/packages/centos/6/noarch/RPMS/nginx-release-centos-6-0.el6.ngx.noarch.rpm` |
| **httpd24** | `curl -s https://repos.fedorapeople.org/repos/jkaluza/httpd24/{epel-httpd24.repo} -o /etc/yum.repos.d/#1` |
| **WandiscoSVN** | `curl -O http://opensource.wandisco.com/scripts/svninstall_centos6_wandisco.sh; sh svninstall_centos6_wandisco.sh` |
| **Elasticsearch** | https://www.elastic.co/guide/en/elasticsearch/reference/current/rpm.html |
| **[Mackerel](https://mackerel.io/ja/docs/entry/howto/install-agent/rpm)** | `curl -fsSL https://mackerel.io/assets/files/scripts/setup-yum.sh `&#124;` sh` |
| **[VirtualBox](https://www.virtualbox.org/wiki/Linux_Downloads)** | `curl -s http://download.virtualbox.org/virtualbox/rpm/el/{virtualbox.repo} -o /etc/yum.repos.d/#1` |
| **[Docker](https://docs.docker.com/engine/installation/linux/centos/)** | `curl -sSL https://get.docker.com/ `&#124;` sh` |

## 各リポジトリーの詳細

### **EPEL** (Extra Packages for Enterprise Linux)
[EPEL/ja - FedoraProject](https://fedoraproject.org/wiki/EPEL/ja)

> EPEL は、 Red Hat Enterprise Linux 向けの高品質なアドオンパッケージであり、CentOS や Scientific Linux のような RHEL からスピンオフしたディストリビューションと互換性のある、Fedora プロジェクトで有志によって作成されたパッケージ

#### インストール
```bash:CentOS7/CentOS6
yum install epel-release
```
```bash:CentOS5
rpm -ivh http://download.fedoraproject.org/pub/epel/5/i386/epel-release-5-4.noarch.rpm
# リダイレクトされない場合は以下
rpm -ivh http://ftp.iij.ad.jp/pub/linux/fedora/epel/5/i386/epel-release-5-4.noarch.rpm
```
`rpm` コマンドでインストールする方法が記載されていることが多いが、CentOS 6 以降は epel-release パッケージが CentOS Extras repository に含まれているので `yum` コマンドでそのままインストール可能。

#### 提供パッケージ一覧
* https://dl.fedoraproject.org/pub/epel/7/x86_64/
* https://dl.fedoraproject.org/pub/epel/6/x86_64/
* https://dl.fedoraproject.org/pub/epel/5/x86_64/

#### インストール時の初期設定

|設定ファイル       |リポジトリー                |有効|
|-----------------|-------------------------|:-:|
|epel.repo        |epel                     | ○ |
|                 |epel-debuginfo           | × |
|                 |epel-source              | × |
|epel-testing.repo|epel-testing             | × |
|                 |epel-testing-debuginfo   | × |
|                 |epel-testing-source      | × |


### **Remi's RPM repository**
[Remi's RPM repository](http://rpms.famillecollet.com/)
比較的新しい PHP を利用したい場合などに利用する。
2006年から Fedora Project の Packager として活動し、2012年から Red Hat 社に在籍するフランス人開発者 Remi Collet 氏が個人でメンテナンスしている。 RHEL の2012年10月以降の PHP のバックポートは全て彼によるもの。

#### インストール
```bash:CentOS7
yum install http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
```
```bash:CentOS6
yum install http://rpms.famillecollet.com/enterprise/remi-release-6.rpm
```
```bash:CentOS5
rpm -ivh http://rpms.famillecollet.com/enterprise/remi-release-5.rpm
```

#### 有効化
```bash
yum install yum-utils
yum-config-manager --enable remi-php70
```

#### 提供パッケージ一覧
* http://rpms.famillecollet.com/enterprise/7/
* http://rpms.famillecollet.com/enterprise/6/
* http://rpms.famillecollet.com/enterprise/5/

#### インストール時の初期設定

|設定ファイル|リポジトリー                     |有効|
|---------------|-------------------------|:-:|
|remi.repo      |remi                     | × |
|               |remi-php55               | × |
|               |remi-php56               | × |
|               |remi-test                | × |
|               |remi-debuginfo           | × |
|               |remi-php55-debuginfo     | × |
|               |remi-php56-debuginfo     | × |
|               |remi-test-debuginfo      | × |
|remi-php70.repo|remi-php70               | × |
|               |remi-php70-debuginfo     | × |
|               |remi-php70-test          | × |
|               |remi-php70-test-debuginfo| × |
|remi-php71.repo|remi-php71               | × |
|               |remi-php71-debuginfo     | × |
|               |remi-php71-test          | × |
|               |remi-php71-test-debuginfo| × |
|remi-safe.repo |remi-safe                | ○ |



### **RepoForge** (旧RPMForge)
[RepoForge Project](http://repoforge.org/)

```bash
yum install http://pkgs.repoforge.org/rpmforge-release/rpmforge-release-0.5.3-1.el`rpm -q --whatprovides /etc/redhat-release --qf '%{version}\n'`.rf.x86_64.rpm
```

#### インストール時の初期設定

|設定ファイル  |リポジトリー     |有効|
|-------------|----------------|:-:|
|rpmforge.repo|rpmforge        | ○ |
|             |rpmforge-extras | × |
|             |rpmforge-testing| × |


### **Webtatic Yum Repository**

[Webtatic Yum Repository](https://webtatic.com/projects/yum-repository/)

```bash:CentOS7
yum install https://mirror.webtatic.com/yum/el7/webtatic-release.rpm
```
```bash:CentOS6
yum install https://mirror.webtatic.com/yum/el6/latest.rpm
```
```bash:CentOS5
rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-5.noarch.rpm
rpm -Uvh http://mirror.webtatic.com/yum/el5/latest.rpm
```

### **The Software Collections ( SCL ) Repository**
https://wiki.centos.org/AdditionalResources/Repositories/SCL
https://access.redhat.com/documentation/en/red-hat-software-collections/

#### インストール
```bash:CentOS7
yum install centos-release-scl
```
```bash:CentOS6
yum install centos-release-SCL
```
```
yum install scl-utils
```
#### 利用例
https://access.redhat.com/documentation/ja-JP/Red_Hat_Enterprise_Linux/7/html/Developer_Guide/scl-utils.html

```
yum install php55
source /opt/rh/php55/enable
```
```bash
scl enable php55 'php -v'
```
```bash
scl enable php55 bash
```
```bash
/opt/rh/php55/root/usr/bin/php -v
```
```bash
service mysql55-mysqld start
```

#### 提供パッケージ一覧
* [List of Software Collections available in SCLo SIG - CentOS Wiki](https://wiki.centos.org/SpecialInterestGroup/SCLo/CollectionsList)
* http://mirror.centos.org/centos/7/sclo/x86_64/
* http://mirror.centos.org/centos/6/sclo/x86_64/
* http://mirror.centos.org/centos/6/SCL/x86_64/


### **MySQL Yum Repository**
公式のMySQL Yumリポジトリーが提供されているので、最新のMySQLをインストールしたい場合に利用したい。
[Download MySQL Yum Repository](https://dev.mysql.com/downloads/repo/yum/)

- CentOS 6.x, 7.x

```bash:mysql57-community-release
yum install https://dev.mysql.com/get/mysql57-community-release-el`rpm -q --whatprovides /etc/redhat-release --qf '%{version}\n'`-9.noarch.rpm
```

- CentOS 5.x

```bash:mysql-community-release
yum install https://dev.mysql.com/get/mysql-community-release-el`rpm -q --whatprovides /etc/redhat-release --qf '%{version}\n'`-7.noarch.rpm
```

#### インストール時の初期設定

|設定ファイル                |リポジトリー                      |有効|
|---------------------------|---------------------------------|:-:|
|mysql-community.repo       |mysql-connectors-community       | ○ |
|                           |mysql-tools-community            | ○ |
|                           |mysql55-community                | × |
|                           |mysql56-community                | × |
|                           |mysql57-community                | ○ |
|                           |mysql80-community                | × |
|                           |mysql-tools-preview              | × |
|mysql-community-source.repo|mysql-connectors-community-source| × |
|                           |mysql-tools-community-source     | × |
|                           |mysql55-community-source         | × |
|                           |mysql56-community-source         | × |
|                           |mysql57-community-source         | × |
|                           |mysql80-community-source         | × |
|                           |mysql-tools-preview-source       | × |

### httpd24
CentOS 6 で Apache 2.4 を Yum リポジトリーからインストールしたい場合。
インストール先が `/opt/rh/httpd24` 配下になり、サービス名は `httpd24-httpd` になるので注意。

```bash:CentOS6
$ curl -s https://repos.fedorapeople.org/repos/jkaluza/httpd24/{epel-httpd24.repo} -o /etc/yum.repos.d/#1
$ yum install httpd24-httpd httpd24-httpd-devel
$ chkconfig httpd24-httpd on
$ ls /opt/rh/httpd24/root/etc/httpd
conf  conf.d  conf.modules.d  logs  modules  run
```

### WandiscoSVN (Subversion 1.8)
デフォルトおよび EPEL, remi のリポジトリーでは Subversion は1.6系しかインストールできない。WANdisco社のリポジトリーを利用すると1.8系がインストール可能となる。

```bash
$ cat << _EOF_ > /etc/yum.repos.d/wandisco-svn.repo
[WandiscoSVN]
name=Wandisco SVN Repo
baseurl=http://opensource.wandisco.com/centos/\$releasever/svn-1.8/RPMS/\$basearch/
enabled=1
gpgcheck=0
_EOF_
$ yum install subversion
```

### IUS
[IUS Community Project](https://ius.io/)

```bash:自動インストール
curl -s https://setup.ius.io/ | sh
```
```bash:手動インストール
yum install https://centos`rpm -q --whatprovides /etc/redhat-release --qf '%{version}\n'`.iuscommunity.org/ius-release.rpm
```
#### 提供パッケージ一覧
https://dl.iuscommunity.org/pub/ius/stable/CentOS/7/x86_64/repoview/

### ELRepo
リリース版ではまだ未対応な最新のハードウェアでも利用可能とするkABI対応ドライバを提供するプロジェクトで、ファイルシステム、グラフィック、ネットワーク、サウンド、WEBカメラやビデオのドライバが含まれる。
また、リリース版よりもドライバのバージョンが進んでいる。[^elrepo]

[ELRepo : HomePage](http://elrepo.org/)

[^elrepo]: http://tsuchinoko.dmmlabs.com/?p=676


```bash:CentOS7
yum install http://www.elrepo.org/elrepo-release-7.0-2.el7.elrepo.noarch.rpm
```
```bash:CentOS6
yum install http://www.elrepo.org/elrepo-release-6-6.el6.elrepo.noarch.rpm
```
#### 提供パッケージ一覧
http://elrepo.org/tiki/Packages


### Atomic Repo
[Atomicorp Archive](https://www.atomicorp.com/channels/)

```bash:自動インストール
curl -s http://www.atomicorp.com/installers/atomic | sh
```

### agr-free RPMs
http://rpm.agresearch.co.nz/

### GhettoForge
http://ghettoforge.org/index.php/Main_Page

### LinuxTECH.NET Repositories
http://pkgrepo.linuxtech.net/el6/

### nux-dextop
http://li.nux.ro/repos.html

```:CentOS7
yum install http://li.nux.ro/download/nux/dextop/el7/x86_64/nux-dextop-release-0-5.el7.nux.noarch.rpm
```
```:CentOS6
yum install http://li.nux.ro/download/nux/dextop/el6/x86_64/nux-dextop-release-0-2.el6.nux.noarch.rpm
```
ffmpeg がパッケージインストールできる。

### RPMfusion Repository
http://rpmfusion.org/

### Samba 4.2 repository
[SerNet EnterpriseSAMBA Portal](https://portal.enterprisesamba.com/)

## リポジトリーの有効無効の設定
CentOS 6 以降では `yum-config-manager` コマンドを使うことで、コマンドだけで変更が可能になる。 `yum-utils` をインストールすると使えるようになる。

```bash
$ yum install yum-utils
$ yum-config-manager --enable remi remi-php56
```

## リンク
* [【個人メモ】CentOS環境に登録するyumリポジトリ - Qiita](http://qiita.com/futoase/items/0ca6b61cb88194c90367)
* [CentOS7.0 yum外部リポジトリまとめ(2015/03/04版) - Qiita](http://qiita.com/m2wasabi/items/57ee6663e5de653870ff)
* [Remiリポジトリを使って最新版のphp等をyumでインストールする - Qiita](http://qiita.com/is0me/items/eb7e9dd823a1dee944d3)
* [php5.5とかphp5.6をインストールする - Qiita](http://qiita.com/ykyk1218/items/c859870ef8dac79f5e1c)
* [Centos5,6,7にEPEL/REMIのyumリポジトリの追加をする。 - Qiita](http://qiita.com/chidakiyo/items/3b81a442dda34d439b42)
* [yumまとめ - Qiita](http://qiita.com/tenbrother/items/96422c7604ecfe990533)
* [CentOSにEPELリポジトリを追加する - Qiita](http://qiita.com/muniere/items/6c4923a070cbbd824f39)
