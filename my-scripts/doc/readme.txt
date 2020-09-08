1) create a new repo on github

2) add my-scripts dir

cd meta-qt5

echo "# meta-qt5 fork" >> README.md

git init

git add .

git commit -m "first commit"

git remote add origin git@github.com:RobertBerger/meta-qt5.git

git push -u origin master

3) use my repo

mv meta-qt5 meta-qt5.ori
git clone git@github.com:RobertBerger/meta-qt5.git

4) add upstream

cd meta-qt5

git remote add official-upstream git://github.com/meta-qt5/meta-qt5

$ git fetch official-upstream

warning: no common commits
remote: Enumerating objects: 103, done.
remote: Counting objects: 100% (103/103), done.
remote: Compressing objects: 100% (68/68), done.
remote: Total 13745 (delta 52), reused 82 (delta 35), pack-reused 13642
Receiving objects: 100% (13745/13745), 3.48 MiB | 5.73 MiB/s, done.
Resolving deltas: 100% (9685/9685), done.
From git://github.com/meta-qt5/meta-qt5
 * [new branch]      daisy             -> official-upstream/daisy
 * [new branch]      dizzy             -> official-upstream/dizzy
 * [new branch]      dora              -> official-upstream/dora
 * [new branch]      dora-next         -> official-upstream/dora-next
 * [new branch]      dunfell           -> official-upstream/dunfell
 * [new branch]      dunfell-next      -> official-upstream/dunfell-next
 * [new branch]      dylan             -> official-upstream/dylan
 * [new branch]      fido              -> official-upstream/fido
 * [new branch]      fido-next         -> official-upstream/fido-next
 * [new branch]      jansa/bison       -> official-upstream/jansa/bison
 * [new branch]      jansa/daisy       -> official-upstream/jansa/daisy
 * [new branch]      jansa/dizzy       -> official-upstream/jansa/dizzy
 * [new branch]      jansa/dunfell     -> official-upstream/jansa/dunfell
 * [new branch]      jansa/fido        -> official-upstream/jansa/fido
 * [new branch]      jansa/jethro      -> official-upstream/jansa/jethro
 * [new branch]      jansa/krogoth     -> official-upstream/jansa/krogoth
 * [new branch]      jansa/master      -> official-upstream/jansa/master
 * [new branch]      jansa/master-5.12 -> official-upstream/jansa/master-5.12
 * [new branch]      jansa/master-5.15 -> official-upstream/jansa/master-5.15
 * [new branch]      jansa/master-py3  -> official-upstream/jansa/master-py3
 * [new branch]      jansa/morty       -> official-upstream/jansa/morty
 * [new branch]      jansa/pyro        -> official-upstream/jansa/pyro
 * [new branch]      jansa/qt5-creator -> official-upstream/jansa/qt5-creator
 * [new branch]      jansa/rocko       -> official-upstream/jansa/rocko
 * [new branch]      jansa/sumo        -> official-upstream/jansa/sumo
 * [new branch]      jansa/thud        -> official-upstream/jansa/thud
 * [new branch]      jansa/warrior     -> official-upstream/jansa/warrior
 * [new branch]      jansa/zeus        -> official-upstream/jansa/zeus
 * [new branch]      jethro            -> official-upstream/jethro
 * [new branch]      jethro-next       -> official-upstream/jethro-next
 * [new branch]      krogoth           -> official-upstream/krogoth
 * [new branch]      krogoth-next      -> official-upstream/krogoth-next
 * [new branch]      master            -> official-upstream/master
 * [new branch]      master-next       -> official-upstream/master-next
 * [new branch]      morty             -> official-upstream/morty
 * [new branch]      morty-next        -> official-upstream/morty-next
 * [new branch]      otavio/master     -> official-upstream/otavio/master
 * [new branch]      pyro              -> official-upstream/pyro
 * [new branch]      pyro-next         -> official-upstream/pyro-next
 * [new branch]      rocko             -> official-upstream/rocko
 * [new branch]      rocko-next        -> official-upstream/rocko-next
 * [new branch]      sumo              -> official-upstream/sumo
 * [new branch]      sumo-next         -> official-upstream/sumo-next
 * [new branch]      thud              -> official-upstream/thud
 * [new branch]      thud-next         -> official-upstream/thud-next
 * [new branch]      warrior           -> official-upstream/warrior
 * [new branch]      warrior-next      -> official-upstream/warrior-next
 * [new branch]      zeus              -> official-upstream/zeus
 * [new branch]      zeus-next         -> official-upstream/zeus-next
 * [new tag]         5.2.1+origin/release  -> 5.2.1+origin/release
 * [new tag]         jansa/test-2013-10-08 -> jansa/test-2013-10-08

$ git branch -a

* master
  remotes/official-upstream/daisy
  remotes/official-upstream/dizzy
  remotes/official-upstream/dora
  remotes/official-upstream/dora-next
  remotes/official-upstream/dunfell
  remotes/official-upstream/dunfell-next
  remotes/official-upstream/dylan
  remotes/official-upstream/fido
  remotes/official-upstream/fido-next
  remotes/official-upstream/jansa/bison
  remotes/official-upstream/jansa/daisy
  remotes/official-upstream/jansa/dizzy
  remotes/official-upstream/jansa/dunfell
  remotes/official-upstream/jansa/fido
  remotes/official-upstream/jansa/jethro
  remotes/official-upstream/jansa/krogoth
  remotes/official-upstream/jansa/master
  remotes/official-upstream/jansa/master-5.12
  remotes/official-upstream/jansa/master-5.15
  remotes/official-upstream/jansa/master-py3
  remotes/official-upstream/jansa/morty
  remotes/official-upstream/jansa/pyro
  remotes/official-upstream/jansa/qt5-creator
  remotes/official-upstream/jansa/rocko
  remotes/official-upstream/jansa/sumo
  remotes/official-upstream/jansa/thud
  remotes/official-upstream/jansa/warrior
  remotes/official-upstream/jansa/zeus
  remotes/official-upstream/jethro
  remotes/official-upstream/jethro-next
  remotes/official-upstream/krogoth
  remotes/official-upstream/krogoth-next
  remotes/official-upstream/master
  remotes/official-upstream/master-next
  remotes/official-upstream/morty
  remotes/official-upstream/morty-next
  remotes/official-upstream/otavio/master
  remotes/official-upstream/pyro
  remotes/official-upstream/pyro-next
  remotes/official-upstream/rocko
  remotes/official-upstream/rocko-next
  remotes/official-upstream/sumo
  remotes/official-upstream/sumo-next
  remotes/official-upstream/thud
  remotes/official-upstream/thud-next
  remotes/official-upstream/warrior
  remotes/official-upstream/warrior-next
  remotes/official-upstream/zeus
  remotes/official-upstream/zeus-next
  remotes/origin/HEAD -> origin/master
  remotes/origin/master

5) use specific upstream branch/commit and make own branch

syntax: git fetch url-to-repo branchname:refs/remotes/origin/branchname

$ git fetch git://github.com/meta-qt5/meta-qt5 dunfell:refs/remotes/origin/dunfell




From git://github.com/Freescale/meta-freescale
 * [new branch]        dunfell    -> origin/dunfell

6) Update from upstream:
git co master
>> git remote -v

official-upstream       git://github.com/Freescale/meta-freescale (fetch)
official-upstream       git://github.com/Freescale/meta-freescale (push)
origin  git@github.com:RobertBerger/meta-freescale.git (fetch)
origin  git@github.com:RobertBerger/meta-freescale.git (push)

>> git fetch official-upstream
remote: Counting objects: 4043, done.
remote: Compressing objects: 100% (1273/1273), done.
remote: Total 4043 (delta 3130), reused 3632 (delta 2727)
Receiving objects: 100% (4043/4043), 721.50 KiB | 402.00 KiB/s, done.
Resolving deltas: 100% (3130/3130), completed with 502 local objects.
From git://git://github.com/Freescale/meta-freescale
   62591d9..e758547  master     -> official-upstream/master
 + 2942327...a382678 master-next -> official-upstream/master-next  (forced update)
   a3fa5ce..6a1f33c  morty      -> official-upstream/morty
---

7) My own branch:
git co master
git co official-upstream/dunfell
git checkout -b 2020-08-28-dunfell
git co master
cd my-scripts
./push-all-to-github.sh

8) apply patches

cd meta-virtualization

git co 2019-09-09-warrior-2.7+

stg init

stg series

stg import --mail ../meta-virtualization-patches/2019-09-09-warrior-2.7+/0001-use-systemd-as-cgroup-manager-for-docker-While-it-s-.patch

import all patches

...

stg series

stg commit --all

git log

git co master

9) push to my upstream

my-scripts/push-all-to-github.sh

