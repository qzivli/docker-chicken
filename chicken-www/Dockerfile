FROM qzivli/chicken-base

RUN chicken-install spiffy

ADD csirc /root/.csirc

# (system "bash")
CMD ["csi", "-q"]
