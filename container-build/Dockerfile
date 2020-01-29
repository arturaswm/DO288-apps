# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

EXPOSE 8080

LABEL io.k8s.description="A basic http server child image, uses onbuild" \
	io.k8s.display-name="apache http server" \
	io.openshift.expose-services="8080:http" \
	io.openshift.tags="apache, httpd"

RUN set -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf

