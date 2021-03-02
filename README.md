# bind9
filter-a plugin to filter out A records if AAAA is present (opposite of filter-aaaa plugin).

Usage:

plugin query "filter-a.so" {
        filter-a-on-v4 yes;
        filter-a-on-v6 yes;
        filter-a { 192.0.2.1; 2001:db8:2::1; };
};
