FROM cobers/drupal
MAINTAINER John nie <80285394@qq.com>
ENV DEBIAN_FRONTEND noninteractive

# Uninstall modules
RUN /etc/init.d/mysql start && \
  vendor/bin/drupal mou -y \
    toolbar 


# Finish
EXPOSE 80 3306 22 443
CMD exec supervisord -n


