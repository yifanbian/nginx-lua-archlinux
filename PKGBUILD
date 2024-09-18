_pfxdir=/opt/openresty
_ngxdir=$_pfxdir/nginx
_cfgdir=$_ngxdir/conf
_tmpdir=/var/lib/openresty
pkgname=openresty
pkgver=1.27.1
pkgrel=1
pkgdesc="A Fast and Scalable Web Platform by Extending NGINX with Lua"
arch=('x86_64')
url="http://openresty.org/"
license=('BSD')
depends=('perl>=5.6.1' 'readline' 'pcre')
makedepends=('rust')
install=$pkgname.install
options=(!purge)
validpgpkeys=(
'B0F4253373F8F6F510D42178520A9993A1C052F8'
)
luajit_version=2.1-20240815
ngx_devel_version=0.3.3
ngx_echo_version=0.63
ngx_coolkit_version=0.2
ngx_set_misc_version=0.33
ngx_srcache_version=0.33
ngx_lua_version=0.10.27
ngx_lua_upstream_version=0.07
ngx_headers_more_version=0.37
ngx_array_var_version=0.06
ngx_memc_version=0.20
ngx_redis2_version=0.15
ngx_stream_lua_version=0.0.15
ngx_lua_resty_core_version=0.1.29
ngx_lua_resty_lrucache_version=0.14
ngx_lua_resty_string_version=0.16
lua_cjson_version=2.1.0.14

source=(http://nginx.org/download/nginx-$pkgver.tar.gz{,.asc}
        luajit2-$luajit_version.tar.gz::https://github.com/openresty/luajit2/archive/v$luajit_version.tar.gz
        ngx_devel_kit-$ngx_devel_version.tar.gz::https://github.com/vision5/ngx_devel_kit/archive/v$ngx_devel_version.tar.gz
        echo-nginx-module-$ngx_echo_version.tar.gz::https://github.com/openresty/echo-nginx-module/archive/v$ngx_echo_version.tar.gz
        ngx_coolkit-$ngx_coolkit_version.tar.gz::https://github.com/FRiCKLE/ngx_coolkit/archive/$ngx_coolkit_version.tar.gz
        set-misc-nginx-module-$ngx_set_misc_version.tar.gz::https://github.com/openresty/set-misc-nginx-module/archive/v$ngx_set_misc_version.tar.gz
        srcache-nginx-module-$ngx_srcache_version.tar.gz::https://github.com/openresty/srcache-nginx-module/archive/v$ngx_srcache_version.tar.gz
        lua-nginx-module-$ngx_lua_version.tar.gz::https://github.com/openresty/lua-nginx-module/archive/v$ngx_lua_version.tar.gz
        lua-upstream-nginx-module-$ngx_lua_upstream_version.tar.gz::https://github.com/openresty/lua-upstream-nginx-module/archive/v$ngx_lua_upstream_version.tar.gz
        headers-more-nginx-module-$ngx_headers_more_version.tar.gz::https://github.com/openresty/headers-more-nginx-module/archive/v$ngx_headers_more_version.tar.gz
        array-var-nginx-module-$ngx_array_var_version.tar.gz::https://github.com/openresty/array-var-nginx-module/archive/v$ngx_array_var_version.tar.gz
        memc-nginx-module-$ngx_memc_version.tar.gz::https://github.com/openresty/memc-nginx-module/archive/v$ngx_memc_version.tar.gz
        redis2-nginx-module-$ngx_redis2_version.tar.gz::https://github.com/openresty/redis2-nginx-module/archive/v$ngx_redis2_version.tar.gz
        stream-lua-nginx-module-$ngx_stream_lua_version.tar.gz::https://github.com/openresty/stream-lua-nginx-module/archive/v$ngx_stream_lua_version.tar.gz
        lua-resty-core-$ngx_lua_resty_core_version.tar.gz::https://github.com/openresty/lua-resty-core/archive/v$ngx_lua_resty_core_version.tar.gz
        lua-resty-lrucache-$ngx_lua_resty_lrucache_version.tar.gz::https://github.com/openresty/lua-resty-lrucache/archive/v$ngx_lua_resty_lrucache_version.tar.gz
        lua-resty-string-$lua_cjson_version.tar.gz::https://github.com/openresty/lua-resty-string/archive/refs/tags/v$ngx_lua_resty_string_version.tar.gz
        lua-resty-cookie.tar.gz::https://github.com/cloudflare/lua-resty-cookie/archive/master.tar.gz
        lua-cjson-$lua_cjson_version.tar.gz::https://github.com/openresty/lua-cjson/archive/refs/tags/$lua_cjson_version.tar.gz
        service
        default
        $pkgname.logrotate
        $pkgname.install
        $pkgname.sh
        )
noextract=()
sha256sums=('54ef91ec8ebcaa486c640c09c92d832eaeaff149b10ee52ef140f407b1b04d1c'
            'SKIP'
            '4275bf97356d713826e7195d1c330568b6089ff1fd4c6954f998e0f60a2baa30'
            '0e971105e210d272a497567fa2e2c256f4e39b845a5ba80d373e26ba1abfbd85'
            '86f6866baf7297d85feb42ff6d9c212d1de696f3314a53d3a41a4b533a67ab01'
            '191f19202e5814996359b66f55b3b32d21d96a47db7295bdb059d6b5a00b08e1'
            'f1ad2459c4ee6a61771aa84f77871f4bfe42943a4aa4c30c62ba3f981f52c201'
            'fd80e59b672e4ff3b4e943740b3facab421c6965226b5934aed16a514baacf47'
            '242d60b97eb7459cd0c0d58083cf7f3195d46181829da45ab8b09a857bb0ed01'
            '2a69815e4ae01aa8b170941a8e1a10b6f6a9aab699dee485d58f021dd933829a'
            'a3dcbab117a9c103bc1ea5200fc00a7b7d2af97ff7fd525f16f8ac2632e30fbf'
            'c949d4be6f3442c8e2937046448dc8d8def25c0e0fa6f4e805144cea45eabe80'
            '8c2bdbe875e4f5225d0778bfb09a2668f9281d7de6218c7b462a7ba2cee06fe8'
            'd255571bcfb9939b78099df39cb4d42f174d789aec8c8e5e47b93942b0299438'
            '6fcf7054f412a19c23c1ac3c0663f42f40bccc907d98c5d1657ae5cab9973ee9'
            'a377fbce78ba10f3ed3a8b5173ea318f8cf8da9d2ab127bb1e1f263078bf7da0'
            'dae9fb572f04e7df0dabc228f21cdd8bbfa1ff88e682e983ef558585bc899de0'
            'a1290ae5f2c7829a9f680d38cb9e6ad3245cfbbe2df9cc65919b3370fdfc2401'
            '2c30af9fcdb75393a738172b50410e93ec817fe61d5421cdd76ba2a20be43edd'
            'bd6bee4ccc6cf3307ab6ca0eea693a921fab9b067ba40ae12a652636da588ff7'
            '39604e1e1caf39f7957aef6f69e54f863d5f9bf0007c25ae8162e892a2dc31b1'
            '3685353f77b7b38c584b73a9b695766ac3123c4d760fb208d5e490ca50b2bb16'
            '4a62b72e3d2d0d520ca789dae6a5664c26647e08681f5405edeeb65da9cebacd'
            'f071e0fd8d0d588f03fcc7db6f3cb3f7ea1b870d3416a0bde142d9aeb839d0f6'
            'bf628aa47fb85f036f250416f13900be61dccac89736434498a80989b16ae85a')
backup=(${_cfgdir:1}/fastcgi.conf
        ${_cfgdir:1}/fastcgi_params
        ${_cfgdir:1}/koi-win
        ${_cfgdir:1}/koi-utf
        ${_cfgdir:1}/mime.types
        ${_cfgdir:1}/nginx.conf
        ${_cfgdir:1}/scgi_params
        ${_cfgdir:1}/uwsgi_params
        ${_cfgdir:1}/win-utf
        etc/logrotate.d/openresty
        etc/default/openresty)

build() {
  # Build LuaJIT
  tmpdir=$(mktemp -d)
  cd "$srcdir/luajit2-$luajit_version"
  make PREFIX=$_pfxdir/luajit
  make install PREFIX=$tmpdir/luajit-build

  # Build nginx
  cd "$srcdir/nginx-$pkgver"
  LUAJIT_LIB=$tmpdir/luajit-build/lib LUAJIT_INC=$tmpdir/luajit-build/include/luajit-2.1 ./configure \
    --prefix=$_pfxdir/nginx \
    --with-cc-opt="-O2 -DNGX_LUA_ABORT_AT_PANIC" \
    --with-ld-opt="-Wl,-rpath,$_pfxdir/luajit/lib" \
    --conf-path=$_cfgdir/nginx.conf \
    --user=http --group=http \
    --add-module=../ngx_devel_kit-$ngx_devel_version \
    --add-module=../echo-nginx-module-$ngx_echo_version \
    --add-module=../ngx_coolkit-$ngx_coolkit_version \
    --add-module=../set-misc-nginx-module-$ngx_set_misc_version \
    --add-module=../srcache-nginx-module-$ngx_srcache_version \
    --add-module=../lua-nginx-module-$ngx_lua_version \
    --add-module=../lua-upstream-nginx-module-$ngx_lua_upstream_version \
    --add-module=../headers-more-nginx-module-$ngx_headers_more_version \
    --add-module=../array-var-nginx-module-$ngx_array_var_version \
    --add-module=../memc-nginx-module-$ngx_memc_version \
    --add-module=../redis2-nginx-module-$ngx_redis2_version \
    --add-module=../stream-lua-nginx-module-$ngx_stream_lua_version \
    --with-file-aio \
    --with-http_stub_status_module \
    --with-http_realip_module \
    --with-http_addition_module \
    --with-http_auth_request_module \
    --with-http_secure_link_module \
    --with-http_random_index_module \
    --with-http_gzip_static_module \
    --with-http_sub_module \
    --with-http_dav_module \
    --with-http_flv_module \
    --with-http_mp4_module \
    --with-http_gunzip_module \
    --with-threads \
    --with-http_ssl_module \
    --with-pcre-jit \
    --with-http_v2_module \
    --with-stream \
    --with-stream_ssl_module \
    --with-stream_ssl_preread_module \
    --without-mail_pop3_module \
    --without-mail_imap_module \
    --without-mail_smtp_module 
  make
  rm -rf $tmpdir
}

package() {
  cd "$srcdir/luajit2-$luajit_version"
  make DESTDIR="$pkgdir" PREFIX="$_pfxdir/luajit" install
  cd "$srcdir/nginx-$pkgver"
  make DESTDIR="$pkgdir" install
  install -Dm644 LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE
  install -d "$pkgdir"/etc/logrotate.d
  install -m644 "$srcdir"/openresty.logrotate "$pkgdir"/etc/logrotate.d/openresty
  install -d "$pkgdir"/etc/default
  install -m644 "$srcdir"/default "$pkgdir"/etc/default/openresty
  install -d "$pkgdir"/$_tmpdir
  install -Dm644 "$srcdir/service" "$pkgdir/usr/lib/systemd/system/openresty.service"
  rm -rf "$pkgdir/var/run"
  install -Dm755 $srcdir/$pkgname.sh $pkgdir/etc/profile.d/$pkgname.sh
  cd "$srcdir/lua-cjson-$lua_cjson_version"
  make PREFIX="$pkgdir/$_pfxdir/luajit" LUA_INCLUDE_DIR="$pkgdir/$_pfxdir/luajit/include/luajit-2.1" install
  cd "$srcdir/lua-resty-core-$ngx_lua_resty_core_version"
  make DESTDIR="$pkgdir" LUA_LIB_DIR="$_pfxdir/luajit/share/lua/5.1" install
  cd "$srcdir/lua-resty-string-$ngx_lua_resty_string_version"
  make DESTDIR="$pkgdir" LUA_LIB_DIR="$_pfxdir/luajit/share/lua/5.1" install
  cd "$srcdir/lua-resty-lrucache-$ngx_lua_resty_lrucache_version"
  make DESTDIR="$pkgdir" LUA_LIB_DIR="$_pfxdir/luajit/share/lua/5.1" install
  cd "$srcdir/lua-resty-cookie-master"
  make DESTDIR="$pkgdir" LUA_LIB_DIR="$_pfxdir/luajit/share/lua/5.1" install
}
# vim:set ts=2 sw=2 et:
