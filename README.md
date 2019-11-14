# ansible-gnmi

[root@compute231 ansible-gnmi]# ansible-playbook srlinux-play.yml 
 [WARNING]: provided hosts list is empty, only localhost is available. Note that the implicit localhost does not match 'all'


PLAY [localhost] *****************************************************************************************************************************************************************

TASK [srlinux-play : show operational state] *************************************************************************************************************************************
changed: [localhost]

TASK [srlinux-play : Display result show version] ********************************************************************************************************************************
ok: [localhost] => {
    "result.stdout_lines": [
        "== getRequest:", 
        "path: <", 
        "  elem: <", 
        "    name: \"interface\"", 
        "    key: <", 
        "      key: \"name\"", 
        "      value: \"mgmt0\"", 
        "    >", 
        "  >", 
        "  elem: <", 
        "    name: \"oper-state\"", 
        "  >", 
        ">", 
        "encoding: JSON_IETF", 
        "", 
        "== getResponse:", 
        "notification: <", 
        "  timestamp: 1573760896576353737", 
        "  update: <", 
        "    path: <", 
        "      elem: <", 
        "        name: \"srl_nokia-interfaces:interface\"", 
        "        key: <", 
        "          key: \"name\"", 
        "          value: \"mgmt0\"", 
        "        >", 
        "      >", 
        "      elem: <", 
        "        name: \"oper-state\"", 
        "      >", 
        "    >", 
        "    val: <", 
        "      json_ietf_val: \"\\\"up\\\"\"", 
        "    >", 
        "  >", 
        ">"
    ]
}

PLAY RECAP ***********************************************************************************************************************************************************************
localhost                  : ok=2    changed=1    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0  