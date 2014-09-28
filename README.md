# Ansible Role: Apache Solr

An Ansible Role that installs Apache Solr on Debian/Ubuntu Linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `vars/main.yml`):

    # Files will be downloaded to this path on the remote server before being moved into place.
    workspace: /root

    # The Apache Solr version to install.
    solr_version: "4.9.0"

    # Java package to install
    solr_java_package: openjdk-7-jre-headless

    # The path where Apache Solr will be installed.
    solr_path: /opt/solr

    # The path where all cores are located
    solr_home_path: /var/data/solr 

    # The name of the group that owns the home path
    solr_home_group: root

## Dependencies

None.

## Example Playbook

    - hosts: solrserver
      roles:
        - { role: solr }

## License

MIT / BSD

