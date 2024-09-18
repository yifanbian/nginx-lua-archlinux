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
'43387825DDB1BB97EC36BA5D007C8D7C15D87369'
'8540A6F18833A80E9C1653A42FD21310B49F6B46'
'573BFD6B3D8FBC641079A6ABABF5BD827BD9BF62'
'9E9BE90EACBCDE69FE9B204CBCDCD8A38D88A2B3'
'D6786CE303D9A9022998DC6CC8464D549AF75C0A'
'7338973069ED3F443F4D37DFA64FD5B17ADB39A8'
'13C82A63B603576156E30A4EA0EA981B66B0D967'
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
sha256sums=('bd7ba68a6ce1ea3768b771c7e2ab4955a59fb1b1ae8d554fedb6c2304104bdfc'
            'SKIP'
            '9e59ec13c301c8b2855838b1248def49ef348a3e7563fabef677431706718145'
            'faa2fcd5168b10764d35081356511d5f84db5c526a1aa4b6add2db94b6853b2b'
            '8af374d29592ef95baee53c91959c7b04927f11304c318a94f0ee140760515a4'
            '191f19202e5814996359b66f55b3b32d21d96a47db7295bdb059d6b5a00b08e1'
            'cd5e2cc834bcfa30149e7511f2b5a2183baf0b70dc091af717a89a64e44a2985'
            '1ffd3e244a52bc2ad31661b038fa20fab3145dea506d97f53c2ac80b55eb38d3'
            'a0a5e616c4a0a32e48899d12242fed5a371f69a85f11ff274a87a2f02f419876'
            '2a69815e4ae01aa8b170941a8e1a10b6f6a9aab699dee485d58f021dd933829a'
            'cf6e169d6b350c06d0c730b0eaf4973394026ad40094cddd3b3a5b346577019d'
            '2c3577265d1d51a2d0646311b9c651520a74455253b6f7a5776af79e9bff5cb1'
            'a42dd56dd6e2144755a127bcd2a6cc1a488258dc5cdb751d6a3e5dd5b6989239'
            'd255571bcfb9939b78099df39cb4d42f174d789aec8c8e5e47b93942b0299438'
            'ecf5c2afd345149cef19bf2e3e196bf1c514ca85e778f853f80a379284b70de1'
            'e416241724ce36ae90dddae8652f8c451e1ad87ebfb3cd62de76985492ef315f'
            '5a9f2e3a292dc9745f267082fc4d5b9bed5ab55f27ea5495986eb2965918e803'
            '77f006a97fd4a3be4a82dcf2d5f1482e399b70fb35454c5b5ad4b97ff1dded0d'
            '5befe684267c9f2e521878adaee2a039e8a66160a21e0ae8614e72a6c9b94aac'
            '14cac5c7a4520b33449a1fc961344556b8b6a2a2c6b739b0e46e3002e6e605bc'
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
