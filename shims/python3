#!/usr/bin/env bash
set -e
[ -n "$PYENV_DEBUG" ] && set -x

program="${0##*/}"

export PYENV_ROOT="/opt/pyenv-build/pyenv2.8.4-openssl365"
SHIM_PATH=${0%/*}
if [[ $SHIM_PATH != "/opt/pyenv-build/pyenv2.8.4-openssl365/shims" ]]; then
  export _PYENV_SHIM_PATH="$SHIM_PATH"
fi
exec "/opt/pyenv-build/pyenv2.8.4-openssl365/libexec/pyenv" exec "$program" "$@"
