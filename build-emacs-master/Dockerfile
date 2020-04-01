FROM olanilsson/autoemacs:build-alpine-3.9

RUN git clone --branch master --single-branch --depth 1 git://git.sv.gnu.org/emacs.git /opt/emacs
RUN cd /opt/emacs && ./autogen.sh
RUN cd /opt/emacs && ./configure --with-modules
RUN make -j8
RUN make install
