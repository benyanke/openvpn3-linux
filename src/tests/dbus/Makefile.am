#  OpenVPN 3 Linux client -- Next generation OpenVPN client
#
#  Copyright (C) 2017 - 2018  OpenVPN Inc. <sales@openvpn.net>
#  Copyright (C) 2017 - 2018  David Sommerseth <davids@openvpn.net>
#
#  This program is free software: you can redistribute it and/or modify
#  it under the terms of the GNU Affero General Public License as
#  published by the Free Software Foundation, version 3 of the
#  License.
#
#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  GNU Affero General Public License for more details.
#
#  You should have received a copy of the GNU Affero General Public License
#  along with this program.  If not, see <https://www.gnu.org/licenses/>.
#

MAINTAINERCLEANFILES = \
	Makefile.in

CLEANFILES = \
        *~

AM_CXXFLAGS = \
	$(OPENVPN3_CORE_CXXFLAGS) \
	$(ASIO_CXXFLAGS) \
	$(CRYPTO_CFLAGS) \
	$(LIBGLIBGIO_CFLAGS) \
	$(LIBJSONCPP_CFLAGS) \
	$(LIBLZ4_CFLAGS) \
	$(LIBUUID_CFLAGS)  \
	-I $(top_srcdir)/src

AM_LDFLAGS = \
	$(CRYPTO_LIBS) \
	$(LIBGLIBGIO_LIBS) \
	$(LIBJSONCPP_LIBS) \
	$(LIBLZ4_LIBS) \
	$(LIBUUID_LIBS)

noinst_PROGRAMS = \
	config-lock-down \
	config-override-selftest \
	conncreds \
	enable-logging \
	fetch-avail-config-paths \
	fetch-avail-session-paths \
	fetch-config \
	fetch-config2 \
	get-acl \
	get-config-overrides \
	getlastlogevent \
	getlaststatus \
	getconnectionstats \
	log-listener \
	log-listener2 \
	logservice1 \
	netcfg-stateevent-selftest \
	set-alias \
	signal-listener \
	statusevent-selftest \
	proc-wait-for \
	proc-wait-for-pid \
	request-queue-client \
	request-queue-client2 \
	request-queue-service

config_lock_down_SOURCES = config-lock-down.cpp

config_override_selftest_SOURCES = config-override-selftest.cpp

conncreds_SOURCES = conncreds.cpp

enable_logging_SOURCES = enable-logging.cpp

fetch_avail_config_paths_SOURCES = fetch-avail-config-paths.cpp

fetch_avail_session_paths_SOURCES = fetch-avail-session-paths.cpp

fetch_config_SOURCES = fetch-config.cpp

fetch_config2_SOURCES = fetch-config2.cpp

get_acl_SOURCES = get-acl.cpp

get_config_overrides_SOURCES = get-config-overrides.cpp

getlastlogevent_SOURCES = getlastlogevent.cpp

getlaststatus_SOURCES = getlaststatus.cpp

getconnectionstats_SOURCES = getconnectionstats.cpp

log_listener_SOURCES = log-listener.cpp

log_listener2_SOURCES = log-listener2.cpp

logservice1_SOURCES = logservice1.cpp


netcfg_stateevent_selftest_SOURCES = netcfg-stateevent-selftest.cpp \
	$(top_srcdir)/src/netcfg/netcfg-stateevent.hpp

set_alias_SOURCES = set-alias.cpp

signal_listener_SOURCES = signal-listener.cpp

statusevent_selftest_SOURCES = statusevent-selftest.cpp

proc_wait_for_SOURCES = proc-wait-for.cpp

proc_wait_for_pid_SOURCES = proc-wait-for-pid.cpp

request_queue_client_SOURCES = request-queue-client.cpp

request_queue_client2_SOURCES = request-queue-client2.cpp

request_queue_service_SOURCES = request-queue-service.cpp
